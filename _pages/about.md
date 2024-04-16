---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

My research focuses on why people harm others. To examine this, I study emotions, antisociality, and psychopathology in children and adolescents. I am also interested in research integrity/reform, R, and science communication. Occassionally I do art.

Seleceted papers
======

*Genetic-environment interactions affect youth antisocial behavior?*

In a longitudinal study (N = 721), we assessed how genetic risk for antisociality (via two polygenetic risk scores; PRSa,c) and hostile environments (school violence, harsh parenting) related to stable and unstable forms of antisocial behavior (nonaggressive conduct problems, physical aggression, social aggression) across adolescence (ages 13, 15, and 17 years).

Harsh parenting, violence at school, and antisocial genetic risk were all independently associated with stable forms of antisocial behavior. We also found a consistent genetic-environment interaction specific to late adolescence:
- Higher genetic risk for antisociality: harsher parenting was associated with increased social aggression (red lines)
- Lower genetic risk for antisociality: harsher parenting was associated with decreased social aggression​ (blue lines)
<br/><img src='/images/PRSfig.png'>
Interestingly, each genetic risk score (PRSa and PRSc) showed the same genetic-environment interaction, despite each explaining separate portions of antisocial behavior. Genetic risk scores were not meaningfully correlated with one another likely due to one being derived from a primarily child sample (PRSc), while the other from a largely adult sample (PRSa). 

*IMPLICATIONS:* Harsher parenting was linked to elevated stable antisocial behaviors across adolescence. However, shifts in social aggression in late adolescence were partially explained by a consistent genetic-environment interaction (~8% of variance).

Late adolescents considered more susceptible to antisociality may respond to harsh parenting by mirroring that emotional hostility when interacting with peers. Alternately, youth less susceptible to antisociality may respond to harsh parenting in the opposite way: reducing their social aggression (i.e., abstaining from emotional bullying, isolating others, damaging relationships). Perhaps those with lower genetic risk for antisociality are more socially sensitive individuals, who withdraw from all types of social interactions (good and bad) when they feel attacked.

These interactions may only emerge in late adolescence as youth overall become better at inhibiting their base impulses, making those that cannot control their behavior easier to identify as socially divergent. More research is needed to test this hypothesis. These findings are also correlational so we cannot say for certain it is the environment that causes these changes in behaviour, it could be the other way around or a third factor.

Together this suggests that youth may respond to the same challenging environment in opposite ways depending on their susceptibility to that stressor. 

Acland, E. L., Pocuca, N., Paquin, S., Boivin, M., Ouellet-Morin, I., Andlauer, T. F. M., Gouin, J. P., Côté S. M., Tremblay R. E., Geoffroy, M. & Castellanos-Ryan, N. (2024). Polygenic risk and hostile environments: Links to stable and dynamic antisocial behaviors across adolescence. Development and Psychopathology, 1-13. https://doi.org/10.1017/S095457942400004X (Open access article). 


Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
