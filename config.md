<!--
Add here global page variables to use throughout your website.
-->
+++
title = "Blog Title"
description = "blog description"
author = "Blog author"
mintoclevel = 2
prepath = "blog"
repo_url = "github-url" # empty if not a repo

# Add here files or directories that should be ignored by Franklin, otherwise
# these files might be copied and, if markdown, processed by Franklin which
# you might not want. Indicate directories by ending the name with a `/`.
# Base files such as LICENSE.md and README.md are ignored by default.
ignore = ["node_modules/", "LanguageTool/", "Manifest.toml", "Project.toml", "LanguageTool.jl", "blog"]

# RSS (the website_{title, descr, url} must be defined to get RSS)
generate_rss = true
website_title = title 
website_descr = description
website_url   = ""
+++

<!--
Add here global latex commands to use throughout your pages.
-->
\newcommand{\R}{\mathbb R}
\newcommand{\scal}[1]{\langle #1 \rangle}
