---
permalink: /
title: "Background"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a hydro-geodesist with a knowledge of hydrological sciences, particularly surface hydrology and wetlands. I have been working as a PhD student in the unit of Water, Permafrost, and Environmental Systems at Stockholm University (SU) since 2019. Prior to that, I did my undergraduate and graduate studies in geomatics and marine geodesy, at the Universities of Tafresh and Tehran in Iran, with a strong focus on both theories and applications of remote sensing. Prior to my PhD journey, I gained valuable insights and expertise in the offshore and onshore industries such as hydrographic and land surveying. However, it was during my PhD that I truly discovered my passion for research, which allowed me to develop my own ideas.

PhD Thesis
======
It was on my very first flight to Stockholm that the high density of surface water bodies over Sweden attracted my attention. That visual inspection from the airplane’s window, I count as my first attempt at remote sensing of the Swedish lakes. During my PhD, I have used optical satellite images to understand water occurrence in deltas and Radar images (SAR) and Radar Altimetry to develop innovative methodologies for lake water level estimation. My PhD research has led to five manuscripts (1 published and 4 under review) that four of which are included in my thesis.
To understand the temporal and spatial variations in surface water occurrence and levels, my thesis addresses three over-arching objectives outlined in Figure 1. The first two objectives relate to a hydrologic analysis of water occurrence and water levels by applying satellite optical imagery, Radar altimetry, and statistical analysis. The third objective seeks to tackle remote sensing methodological challenges by using D-InSAR over Swedish lakes. Figure 1 illustrates the structure of my thesis based on the objectives' categories (Hydrologic analysis or Method Development) and the type of satellite sensors (Radar or optical) employed in the methodology of each paper. The study area of the first paper is the Selenga River Delta, situated in East Siberia, and the three subsequent papers focus on Swedish lakes (Figure 1).
Besides research articles, I am developing a comprehensive data product of water levels in approximately 1000 lakes in Sweden, which I expect to be of high interest to the Swedish Meteorological and Hydrological Institute, among other stakeholders.

Figure 1: The structure of my PhD thesis regarding the main focus, the type EO data used in each study, and the case studies.
![Thesis structure](/images/thesis.png)

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
