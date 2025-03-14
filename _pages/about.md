---
permalink: /
title: Carlos Mora Sardiña
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a PhD candidate at the University of California, Irvine, specializing in computational science and engineering. My research interests lie within the fields of machine learning, data fusion and uncertainty quantification. In my work, I develop probabilistic machine learning methods to model complex systems across various scientific and engineering domains. You can find my publications [here](https://cmorasar.github.io/publications-talks/). Additionally, I am grateful to have been awarded with the Balsells fellowship. 

Prior to my PhD, I graduated in aerospace engineering with honors from the Polytechnic University of Catalonia. 

## Recent news
- December 2024: I successfully defended my candidacy exam! My PhD thesis, titled _Integrating Deep Learning with Gaussian Processes for Scientific Computing_, will explore innovative ways to combine these machine learning methods for advancing scientific computing. 
- November 2024: my paper _Operator learning with Gaussian processes_ is now [available](https://www.sciencedirect.com/science/article/pii/S0045782524008351) in Computer Methods in Applied Mechanics and Engineering.
- October 2024: my paper _A gaussian process framework for solving forward and inverse problems involving nonlinear partial differential equations_ has been [published](https://link.springer.com/article/10.1007/s00466-024-02559-0) in Computational Mechanics.
- October 2024: I gave a [talk](https://www.youtube.com/watch?v=yFAxA6vPECA&t=3s) at the CRUNCH seminar on neural operators and Gaussian Processes for operator learning. 
- September 2024: new preprint [available](https://arxiv.org/abs/2409.04538) on a general framework for operator learning via Gaussian Processes.
- August 2024: new preprint [available](https://arxiv.org/abs/2401.03492) where we develop a meshfree topology optimization method with physics-informed Gaussian Processes.
- July 2024: the paper _GP+: A Python library for kernel-based learning via Gaussian processes_ is now [available](https://www.sciencedirect.com/science/article/pii/S0965997824000930) in Advances in Engineering Software.

<!--
May 2024: I presented my research on _Operator learning via neural networks with kernel-weighted corrective residuals_ at EMI/PMC 2024.
 January 2024: new preprint [available](https://arxiv.org/abs/2401.03492) on a novel machine learning method for PDE solving.
- December 2023: new preprint [available](https://arxiv.org/abs/2312.07694) on _GP+: A Python Library for Kernel-based learning via Gaussian Processes_.
- October 2023: my paper _Probabilistic neural data fusion for learning from an arbitrary number of multi-fidelity data sets_ has been [published](https://www.sciencedirect.com/science/article/pii/S0045782523003316) in Computer Methods in Applied Mechanics and Engineering.
- July 2023: I presented my work on _Data Fusion Under Multiple Uncertainty Sources via Multi-Fidelity Bayesian Networks_ at the 17th U.S. National Congress on Computational Mechanics.
- July 2023: I gave a talk on _Probabilistic neural data fusion for learning from an arbitrary number of multi-fidelity data sets_ at the Sandia Machine Learning and Deep Learning Workshop.

 A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

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
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
