<!--
Add here global page variables to use throughout your website.
-->
+++
author = "César López"
mintoclevel = 2

# Add here files or directories that should be ignored by Franklin, otherwise
# these files might be copied and, if markdown, processed by Franklin which
# you might not want. Indicate directories by ending the name with a `/`.
# Base files such as LICENSE.md and README.md are ignored by default.
ignore = ["node_modules/"]

# RSS (the website_{title, descr, url} must be defined to get RSS)
generate_rss = true
website_title = "ArduFree"
website_descr = "Curso de arduino básico"
website_url   = "https://ceesar-lopez.github.io/cursoarduino/"
+++

<!--
Add here global latex commands to use throughout your pages.
-->
@def prepath="cursoarduino"
\newcommand{\R}{\mathbb R}
\newcommand{\scal}[1]{\langle #1 \rangle}
