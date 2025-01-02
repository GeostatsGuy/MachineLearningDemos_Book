### Applied Machine Learning in Python: a Hands-on Guide with Code

Michael J. Pyrcz, Professor, The University of Texas at Austin 

[Twitter](https://twitter.com/geostatsguy) | [GitHub](https://github.com/GeostatsGuy) | [Website](http://michaelpyrcz.com) | [GoogleScholar](https://scholar.google.com/citations?user=QVZ20eQAAAAJ&hl=en&oi=ao) | [Book](https://www.amazon.com/Geostatistical-Reservoir-Modeling-Michael-Pyrcz/dp/0199731446) | [Geostatistics e-book](https://geostatsguy.github.io/GeostatsPyDemos_Book) | [YouTube](https://www.youtube.com/channel/UCLqEr-xV-ceHdXXXrTId5ig)  | [LinkedIn](https://www.linkedin.com/in/michael-pyrcz-61a648a1)

By Michael J. Pyrcz <br />
&copy; Copyright 2024.

This e-book provides an accessible, online version, a new vehicle to share my **Machine Learning Graduate Course** at The University of Texas at Austin, that includes, 

* **Well Documented Demonstration Python Workflows** - almost half the lecture time is spend with these workflows from my [MachineLearningDemos](https://github.com/GeostatsGuy/MachineLearningDemos) GitHub repository, that includes well-documented demonstration Python Jupyter workflows for many common machine learning workflows. One goal of this e-book is to share this content beyond the GitHub users, often only the experts and developers - to reach and help more people!

* **Course Notes** - I'm also making an effort to continue adding more of the course notes into this e-book, to provid even more coverage of theory and implimentation details. 

* **Interactive Python Dashboards** - I have a lot of interactive Python dashboards that I use in my classes that I will continue to explain and cite in this e-book to help you get the entire in-class experience. These are all available in my [DataScienceInteractivePython](https://github.com/GeostatsGuy/DataScienceInteractivePython) GitHub repository.

* **Recorded Lectures** - there are many thousands of views of my lectures every month on [YouTube channel](https://www.youtube.com/@GeostatsGuyLectures), but many of those people are not on GitHub. I will add links to this e-book to support them. Also, the YouTube channel can enhance the e-book experience, read the book and drop by to hear my explanations. 

```{admonition} Welcome!
:class: remove-from-content-only

The scope of this e-book is to teach the application of machine learning in Python, for those new to machine learning I provide and overview of theory and links to my recorded lectures for a deeper dive, and for those experienced practitioners I provide example and enhanced workflows and visualizations that you can implement. 
```

This is my second effort to convert one of my GitHub repositories of well-documented Python workflows into an online, accessible e-book. 

* For those interested in spatial data analytics and geostatistics, I welcome you to visit my other e-book, [Applied Geostatistics in Python: a Hands-on Guide with GeostatsPy](https://geostatsguy.github.io/GeostatsPyDemos_Book/intro.html){cite}`pyrczappliedgeostats2024`. 

The great response to this e-book from students and working professionals all over the world motivated me to compile, build and release this e-book. The original repository for the workflows in this book are found at [MachineLearningDemos: Python Machine Learning Demonstration Workflows Repository](https://github.com/GeostatsGuy/MachineLearningDemos) {cite}`pyrczMLdemos2024`, but rest assured every chapter in this book is a Jupyter Notebook or Jupyter Lab .ipynb file that may be downloaded and run locally. All I ask is that you retain my authorship and cite the source when my work is used. My motivation is to attract more people to all of the resources that I share online! Please consider citing and linking these resources in your work.

```{admonition} Cite this e-Book as:
:class: remove-from-content-only

Pyrcz, M.J., 2024, Applied Machine Learning in Python: a Hands-on Guide with Code, https://geostatsguy.github.io/MachineLearningDemos_Book. 
```

```{admonition} Cite the MachineLearningDemos GitHub Repository as:
:class: remove-from-content-only

Pyrcz, M.J., 2024, MachineLearningDemos: Python Machine Learning Demonstration Workflows Repository (0.0.1). Zenodo. [![DOI](https://zenodo.org/badge/862519860.svg)](https://zenodo.org/doi/10.5281/zenodo.13835312)
```

The ultimate source for the content in this e-book is my semester-long Machine Learning graduate course, so I have made scope decisions based on the educational narrative in my course. 

* I believe that 80\% or more of any data science is data prepartion so I spend 1/3 of the course on workflow design, probability concepts, data preparation and feature engineering before we turn on any machines

* I spend a lot of time on simple machines, like linear regression and the regularized variants to teach fundamental theory

* I step through specific methods to build up concepts, for example, $L^2$ vs $L^1$ norms, regularization, convolution, bootstrap and bagging, Bayesian approaches, etc.

* I have chapters on deep learning that will be added shortly.

I made an effort to order the chapters to build up the concepts of machine learning, from feature engineering, through inferential machine learning and up to predictive machine learning. The predictive machine learning is ordered to start with linear regression, introduce hyperparameter tuning with ridge regression, introduce basis expansion with polynomial regression, integrate Bayesian methods with Bayesian linear regression, demonstrate lazy vs. eager learning with k-nearest neighbours, present ensemble methods with trees, etc. 

* If you work through the chapters in order you will benefit from this "scaffolding"" and "spiraling" approach to education that I like to apply in all of my courses.

* Nevertheless, each chapter is designed to be a stand-alone resource, in most cases you could readily plug and play your own dataset. Remember to cite the e-book and repos and bring me a breakfast taco if you pass through Austin!

This e-book is not a general introduction to statistics nor is it a comprehensive treatment of machine learning. 

* For a deeper dive into the theory and practice built on fundamental probability and statistics follow the links at the top of each chapter to my recorded lectures on my [Machine Learning Lecture Series](https://www.youtube.com/playlist?list=PLG19vXLQHvSC2ZKFIkgVpI9fCjkN38kwf) {cite}`pyrczyoutube` of my YouTube channel.  

* Of course there are excellent books for machine learning theory, one of my favourites is [The Elements of Statistical Learning: Data Mining, Inference, and Prediction](https://www.amazon.com/Elements-Statistical-Learning-Prediction-Statistics/dp/0387848576/ref=sr_1_1?crid=219UH54M8MIS6&dib=eyJ2IjoiMSJ9.fh_JG0GOjaLD32XrqN8uJE0bBbEVgutMStZUYLHACzr8YEzjV2ommtSpLcI0ed8OflRxA4AgTUEYl4S8Y4ICbP3s2OkSR8EaSxk8OHLwyavIw52GFVGGSJpyX9Y7BNipvmjdb8VgidS9njUPpDwpl1CmpD0BTb8LtbTHm8nCXBQT0W21r5H0DU84tHqrT0AQUUBb2fA9DMIdAJGqdFp1yssN1rXciwATn5v4juV5TiA.nGxoUTS2l564x_D3GUdkwt-QUKt8be_WRfy8eJPgjkQ&dib_tag=se&keywords=machine+learning+statistical+learning&qid=1727204107&sprefix=machine+learning+statistical+learning%2Caps%2C119&sr=8-1) {cite}`statlearning2009`.

```{admonition} Linked Recorded Lectures are Available
:class: remove-from-content-only

For a deeper dive into the theory and practice of geostatistics follow the links at the top of each chapter to my recorded YouTube lectures.
```
Just in case you are interested, my YouTube channel includes 3 complete courses:

1. [Data Analytics and Geostatistics Course](https://youtube.com/playlist?list=PLG19vXLQHvSB-D4XKYieEku9GQMQyAzjJ&si=MzTdgS7IfHEhvF4Q) {cite}`pyrczyoutube`
2. [Spatial Data Analytics Course](https://youtube.com/playlist?list=PLG19vXLQHvSDUmEOmBoaxGbFAbvaLdfx4&si=Pd9bNQLVFZ9Yqz6-)
3. [Machine Learning](https://youtube.com/playlist?list=PLG19vXLQHvSC2ZKFIkgVpI9fCjkN38kwf&si=tfOVljWgWiduwGYl)

along with additional lecture series including:

1. [Data Science Interactive Python Demonstrations](https://youtube.com/playlist?list=PLG19vXLQHvSDy26fM3hDLg3VCU7U5BGZl&si=FB2UoSfJrzjwcKAS) - walk-throughs for many of my interactive Python data science dashboards
2. [Data Science Basics in Python](https://youtube.com/playlist?list=PLG19vXLQHvSAufDFgZEFAYQEwMJXklnQV&si=FN_PZ9C9GdJlHxNv) - basics like loading and visualizing data, prerequisites for this e-book
3. [Random Talks](https://youtube.com/playlist?list=PLG19vXLQHvSDyiLrXpqPV8bUMRvOCHiUZ&si=kCApGUp2xPMu6R7Z) - some of my talks on topics such as data analytics, geostatistics and machine learning, and even talks titled, "Choosing Between Industry and Academia", and "How to Have a Happy and Successful Career". 


#### Table of Contents

```{tableofcontents}
```

#### Recent Updates

Here's some highlights from recent updates to this e-book:

##### What's New with Version 0.0.1

* this is the first release. Thank you for joining in early! Sorry, there are many minor formatting issues that I will resolve over the next couple of months. I welcome feedback with errata. I appreciate any assistance. 
* I will be looking at practical methods to integrate my [Interactive Educational Data Science Python Dashboards](https://github.com/GeostatsGuy/DataScienceInteractivePython) interactive dashboards {cite}`pyrczdemos2021`, and more from my [Machine Learning Lecture Series](https://youtube.com/playlist?list=PLG19vXLQHvSC2ZKFIkgVpI9fCjkN38kwf&si=tfOVljWgWiduwGYl) {cite}`pyrczyoutube`.

##### What's New with Version 0.0.2

* added new sections for feature engineering, machine learning concepts overview chapter, and a glossary!
* I'm making efforts to catch and correct error, links, spelling and grammar

#### Motivation for Open Educational Content

There is more to be done, yet I am excited to compile all this content into an accessible format, linked to lectures and with repeatable code. My goal is to help people get started or to improve their application of machine learning. With an e-book, I realize my dream of sharing educational content with:

* **living documents**, I will continuously make improvements and add new content over time, so send me suggestions and errata and return often!
* **repeatable results**, all examples and plots show the code and anyone can reproduce all the results! The code is immediately downloadable, and all data are online available.
* **links**, for rapid access to all associated resources, bringing together all of my educational content.
* **no pay wall**, for anyone around the world to access my content.

For me, this is a wonderful vehicle to combine and share all my educational content. Yes, thousands can follow and mirror my workflows on GitHub, but the e-book will share this content much more widely. I see this with my YouTube channel with tens of thousands of subscribers and as many views per month vs. my GitHub account with about 3,300 following. Accessible and actionable educational content is my personal mantra.

Some might wonder, why does Michael do this? Check out my story and you will learn that education changed my life. I grew up in a low income family in a small town in Canada. In middle school (junior high for my Canadian friends), I delivered newspapers for over a year to save up for my first computer that our school guidance councilor helped me buy at a local used computer store (a Commodore Amiga 1000). A random engineering student talked to me in a gas station late one cold evening and that got me interested in an university education. Education changed my life, so it is my mission to share all my university educational content in that hope that I may lift someone else as I was lifted. 

Before we get started, here's more information about the associated repository, the source of the workflows for this e-book.

#### MachineLearningDemos Repository

The [MachineLearningDemos: Python Machine Learning Demonstration Workflows Repository](https://github.com/GeostatsGuy/MachineLearningDemos){cite}`pyrczMLdemos2024` is the ultimate source of content for this e-book and hosts more than 20 well-documented demonstration workflow for common machine learning. 

* utilizing synthetic data from my [GeoDataSets](https://github.com/GeostatsGuy/GeoDataSets) repository
* small and often 2D examples for fast run times and ease of interpretation
* often used and cited in my courses for repeatable educational content

Common machine learning workflows that are included:

* multivariate analysis
* feature selection
* feature transformations
* cluster analysis
* principal component analysis
* linear regression
* ridge regression
* LASSO regression
* Bayesian linear regression
* naive Bayes classification
* polynomial regression
* k-nearest neighbours
* decision trees
* bagging trees and random forest
* gradient boosting
* support vector machines

I have many other machine learning and data science workflows in my other repositories. As I prepare these for this e-book I will add them to this repository. Let me know if there are other topics of interest.

#### Data Science Interactive Python Repository

One of my favourite things to do is to build out Python interactive dashboards to support my lectures. I think it is awesome to teach a concept and then to get the students to open a dashboard and rapidly try it out, i.e., to play with the system! What motivates this?

* **I'm a visual learner**, yes I understand the math and systems, but seeing them in action is really helpful to me. I know that many are like me.
* **One of the best way to answer questions in class**. A student asked, what do principal component loadings look like? That evening I made a really cool dashboard with one input, amount of correlation between 3 features with another one independent. The outputs included the principal component loadings and variance explained by each principal component. It showed so much, including conservation of variance, and component one as a mixture of the three correlated features as the correlation increased.
* I like to code and I love to make data science displays. **I really like doing this** and I left industry to give back and have fun.

For now I will add links to these interactive dashboards. In the future I would like these to be included in the e-book. I don't see a way to do that at this point.

#### Running the Workflows

You can use this e-book, i.e., read and review the workflows, without ever running the code. I recommend that you run the code yourself to cement the concepts. To do this you only need to install the required Python packages. The good news is that I generally use the common Python packages curated and available through [Anaconda](https://www.anaconda.com/download). There will be a couple of additional packages to install including, 

* **geostatspy** - my spatial data analytics and geostatistics package for some data transformations and visualization
* **pyvista** - 3D grid visualization
* **astropy** - sparse data convolution
* **shap** - Shapley values for explainable machine learning and feature ranking

These packages can all be installed with:

````python
pip install [package_name]
````

from a terminal window. I like to launch the terminal window from Anaconda Navigator from the 'Environments' tab and left click the green arrow and select 'Open Terminal'. This will ensure that the package is installed in the correct location. After teaching 100s of students and seeing many issues, this is my suggestion for the safest way to install Python packages. 


#### Suggestions for Using this e-book

This is a topical approach to the hands-on application of geostatistics. Each chapter stands alone and covers a unique demonstration or workflow using GeostatsPy. Want to rank your features? Want to perform cluster analysis? Want to train and tune a random forest model? Open up the respective chapter and walkthrough the example with all requisite steps, including data loading, data visualization and modeling steps, with all codes available and explained through text and comments and the results shown. In fact, I want the extra mile to show as much as possible with graphical outputs with efficient figures. While doing this, you can go to the linked lecture(s) to fill in any gaps in your knowledge and then download and update the workflow for your application, please remember to cite the e-book in your work, so that others will see and use this resource! Remember, that this content is for educational purposes only and I do not provide any guarantees. There may be errors in the codes, there may be issues with your case that invalidate the assumptions of the e-book's workflows. It is up to you to evaluate your results.

```{warning}
If you adopt any workflows from this e-book you must check your own work.
```

#### Want to Work Together?

I hope this content is helpful to those that want to learn more about subsurface, spatial modeling, data analytics and geostatistics. Students and working professionals are welcome to participate. I'm happy to collaborate with your organization.

* Want to invite me to visit your company for training, mentoring, project review, workflow design and / or consulting? I'd be happy to drop by and work with you! I am a cofounder of a data science education company.

* Interested in partnering, supporting my graduate student research or my Subsurface Data Analytics and Machine Learning consortium (co-PIs including Profs. Foster, Torres-Verdin and van Oort)? My research combines data analytics, stochastic modeling and machine learning theory with practice to develop novel methods and workflows to add value. We are solving challenging subsurface problems!

* I can be reached at mpyrcz@austin.utexas.edu.

I'm always happy to discuss,

*Michael*

Michael Pyrcz, Ph.D., P.Eng. Professor, Cockrell School of Engineering and The Jackson School of Geosciences, The University of Texas at Austin

#### More Resources Available at: [Twitter](https://twitter.com/geostatsguy) | [GitHub](https://github.com/GeostatsGuy) | [Website](http://michaelpyrcz.com) | [GoogleScholar](https://scholar.google.com/citations?user=QVZ20eQAAAAJ&hl=en&oi=ao) | [Book](https://www.amazon.com/Geostatistical-Reservoir-Modeling-Michael-Pyrcz/dp/0199731446) | [YouTube](https://www.youtube.com/channel/UCLqEr-xV-ceHdXXXrTId5ig)  | [LinkedIn](https://www.linkedin.com/in/michael-pyrcz-61a648a1)