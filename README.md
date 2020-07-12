# What is Internationally-Unrelated?

The Internationally Unrelated site is a blog for my friend group from my graduate cohort to talk about all things public policy and international relations. The website is currently in its infancy, and does not contain any true posts as of yet because many of us are in the midst of career transitions. As we reach stability, this site aims to become the location of fruitful analyses, exaggerated political quips, and potentially a collaborative space to build our data footprints and host portfolio pieces.

All portions of the website currently hosted, including even the directory captions and home icon, are test data until we begin producing our own content. The included “Hello R Markdown” and “A Plain Markdown Post” articles are actually authored by Yihui Xie, creator of Blogdown, and are left as a reference point for other members of the friend cohort to reference as they begin to create their first entries. 

While not complete with any meaningful content at this point, the website is operational, should you wish to adventure over and play around with the test pieces. 

Our website is located at: https://internationally-unrelated.netlify.app/

# How is the Website Constructed?

This website was created using the R Blogdown library. This incredible library abstracts away a considerable amount of the work needed to build and host a static website and allows the user to, if they wish, attempt to build a website entirely within RStudio using Blogdown and Shiny functions. The contents of the website are then hosted in a git repository, which can be pointed to for Netlify to generate the site.

Though for some specific stylistic and content related pieces, it was easier for me to produce my own TOML and HTML files from scratch where I was unable to generate them with Blogdown’s functions, I am far from an expert on every moving piece that this package generates for the user. I will however, for the reader’s sake, attempt to give a brief overview of the contents of each folder included and their purpose within the context of this project.

For more reading, I recommend the book "blogdown: Creating Websites with R Markdown" by Yihui Xie, Amber Thomas, and Alison Presmanes Hill:

https://bookdown.org/yihui/blogdown/

And the Blogdown github hosted by Yihui Xei: 

https://github.com/rstudio/blogdown

<br/>

# Contents of the Website

<br/>

### Content

Here lays the markdown files used to create the posts that you see rendered on the site, as well as the html versions of the markdowns after they are knit. Generally speaking, the markdowns and html files *should be* identical, though I manually edit the html files after knitting to produce the content that I would like. Therefore, if you are interested in viewing the website’s visible content, I recommend opening the html versions of the files. 

Also for simplicity’s sake with declaring pathways, I have included a test csv in this folder. See the *2020-06-06-test-file* to view it rendered in a markdown plot with an accompanying regression. The website seems to function well enough with the data sources included here, though it is poor coding practice to junk up a folder with multiple purposes like this, so I may need to relocate the raw data once the website actually sees use.

### Public

This folder is the one that Netlify actually points to for generating the content of the website. This folder contains all of the generated portions of the website from the posts, beginning with folders for all of the posts (containing the same content as the above *Content* folder) and also contains folders for the website theme. 

The theme used for this website is the automatically generated theme, Hugo-Lithium, which serves the purposes of this website well. You will find thematic content and metadata that Blogdown generates in the css, fonts, js, and tags folders.

Also in this folder you will find the podcast(s) folder(s), which I created to fork a separate list of posts from the default theme. My group was looking to add a section to the website where two of them could create a weekly podcast, so I generated a second TOML file and created a directory where they can begin hosting there. Navigating to the currently named *Beevis & Butthead* section of the website will now populate this new list of content. The *podcasts.toml* file is the one created to perform this action.

The *sitemap.xml* is an auto-updated xml file that passes the content of the website to Netlify. 

### Static

This is a folder contains all of the images used and referenced on the website.

### **Themes**
This folder contains the code that generated the Hugo-Lithium theme. I recommend every viewer of this repository to take a peak in here and see the impressive code produced by Jonathan Rutheiser (under MIT) that created this website.
