# Customized R Interaction Plots using Mplus Output

This vignette is to help those who: 
  1. Use a Mac so they cannot create an interaction plot using Mplus, and
  2. Those who want to customize interaction plots using their Mplus output

## Step 1: Create an interaction plot file in Mplus 

Here is example code for doing this using a path model with skewed observed variables and missing data (i.e., leading to the use of the mlr estimator). This can be adapted to other analyses/models as well, see latent variable example [here](https://www.statmodel.com/download/Latent%20variable%20interaction%20LOOP%20plot.pdf).

```diff

TITLE:	Interaction Plot; 

DATA:	FILE IS data.csv; ! Load data
VARIABLE:	
  NAMES ARE
    id pred mod out; ! Name variables in dataset

  USEVARIABLES ARE
    pred mod out; ! Choose variables that will be included in model

  Missing are all (-99); ! Specify what value indicates missing data
  idvariable = id; ! Specify which variable refers to participant ID if relevant

ANALYSIS: estimator = mlr; ! This specifies that the model will estimate sem model using full information maximum likelihood with robust standard errors

DEFINE: ! Standardize or center variables, then create an interaction term
  STANDARDIZE pred mod;
  pred_mod = pred*mod;

MODEL: ! Specify the model and label the predictor as b1, moderator as b2, and interaction as b3
  out on 
	  pred (b1)
	  mod (b2)
	  pred_mod (b3)
	  ;
	
 pred mod pred_mod; ! Allow predictors to covary and estimate missing data

OUTPUT:
  TECH1 tech4;
  STANDARDIZED CINTERVAL;

MODEL CONSTRAINT: ! Specify your plot (here variables are standardized so 1 is equavalent to 1 SD)
  PLOT(lowmod highmod);
  LOOP(pred,-2,2,0.1); ! x-axis will show predictor between + and - 2 SDs at 0.1 increments 
  lowmod = (b1+b3*(-1))*pred+b2*(-1); ! Plot line at 1 SD below the mean of the moderator
  highmod = (b1+b3*(+1))*pred+b2*(+1); ! Plot line at 1 SD above the mean of the moderator

PLOT: TYPE IS PLOT2;
	
```
Running this code should automatically create a .gh5 file in the folder your code is saved.

