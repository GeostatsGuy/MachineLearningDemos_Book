### Machine Learning Concepts

[Twitter](https://twitter.com/geostatsguy) | [GitHub](https://github.com/GeostatsGuy) | [Website](http://michaelpyrcz.com) | [GoogleScholar](https://scholar.google.com/citations?user=QVZ20eQAAAAJ&hl=en&oi=ao) | [Geostatistics Book](https://www.amazon.com/Geostatistical-Reservoir-Modeling-Michael-Pyrcz/dp/0199731446) | [YouTube](https://www.youtube.com/channel/UCLqEr-xV-ceHdXXXrTId5ig)  | [Applied Geostats in Python e-book](https://geostatsguy.github.io/GeostatsPyDemos_Book/intro.html) | [Applied Machine Learning in Python e-book](https://geostatsguy.github.io/MachineLearningDemos_Book/) | [LinkedIn](https://www.linkedin.com/in/michael-pyrcz-61a648a1)

Chapter of e-book "Applied Machine Learning in Python: a Hands-on Guide with Code". 

Cite as: Pyrcz, M.J., 2024, Applied Machine Learning in Python: a Hands-on Guide with Code, https://geostatsguy.github.io/MachineLearningDemos_Book. 

By Michael J. Pyrcz <br />
&copy; Copyright 2024.
This chapter is a summary of **Machine Learning Concepts** including:

* Statistics and Data Analytics
* Inferential Machine Learning
* Predictive Machine Learning
* Machine Learning Model Training and Tuning

**YouTube Lecture**: check out my lecture on [Introduction to Machine Learning](https://youtu.be/zOUM_AnI1DQ?si=Gi2KZTfPa5xQ2Qb6). For your convenience here's a summary of salient points.

#### Motivation for Machine Learning Concepts

You could just open up a Jupyter notebook in Python and start building machine learing models. You could use one line of code like this,

````python
neigh = KNeighborsRegressor(weights = weights,n_neighbors=n_neighbours,p = p).fit(X_train,y_train) 
````

et voila, you have a trained predictive machine learning model that could be applied to make predictions for new cases. But, is this a good model? How good is it? Could it be better? Without knowledge about basic machine learning concepts we can't answer these questions. This chapter provides you with the basic knowledge to answer these questions and to make better, more reliable models. Let's start with some definitions.

#### Big Data

How do you know if you work with big data? The criteria for big data are these 'V's, if you answer yes for atleast some of these, then you are working with big data:

* **Volume**: many data samples, difficult to handle and visualize

* **Velocity**: high rate collection, continuous relative to decision making cycles

* **Variety**: data form various sources, with various types and scales

* **Variability**: data acquisition changes during the project

* **Veracity**: data has various levels of accuracy 

I find that most subsurface engineers and geoscientists answer yes to all of these questions. So I say that wey has been big data long before tech learned about big data. In fact, I state that we in the subsurface resource industries are the original data scientists. Consider the history of Danie Krige working in the deep gold mines of South Africa in the 1950's. He developed statistical, spatial data-driven models to predict gold grades and the impact specific mining unit (SMU), the volume that the mining can selectively extract. 

#### Data Science

If no one else has said this to you, let me have the honor of welcoming you to the fourth paradigm for scientific discovery, data-driven scientific discovery or just data science.


To understand the fourth paradigm let's first consider the previous three pardigms. Here's all of the paradigms:

| 1st Paradigm Empirical Science | 2nd Paradigm Theoretical Science | 3rd Paradigm Computational Science | 4th Paradigm Data Science | 
|--------------------------------|----------------------------------|------------------------------------|---------------------------|
| Experiments                    | Models and Laws                  | Numerical Simulation               | Learning from Data        |
| 430 BC Empedocles proved air has substance | 1011 AD al-Haytham Book of Optics | 1942 Manhattan Project | 2009 Hey et al. Data-Intensive Book |
| 230 BC Eratosthenes measure Earth’s diameter | 1687 AD Newton Principia | 1980 – Global Forecast System (GFS) | 2015 AlphaGo beats a professional Go player |

Of course, we can argue about the boundaries, i.e., when did the paradigms begin? Certainly the Mesopotamians (4000 BC - 3500 BC) conducted experiments that supported their development of the wheel, plow, chariot, weaving loom, and irrigation and we trace the development of artificial neural networks to McColloch and Pitts in 1943. The adoption of a new scientific is a major societal shift that has not occured uniformly around the globe. 

So what caused the first paradigm to start some time between 1943 and 2009? The fundamental mathematics of data driven models has been available for a long time consider the following mathematical and statistical developments in history:

* **Calculus** - Isaac Newton and Gottfried Wilhelm Leibniz independently developed the math to find minimums and maximums during the 1600s with "Methods of Fluxions" 1671 (published posthumously in 1736), and with "Nova Methodus pro Maximis et Minimis" published in 1684.
* **Bayesian Probability** - introduced by Reverend Thomas Bayes with Bayes' Theorem enshrined in "An Essay Towards Solving a Problem in the Doctrine of Chances" published posthumously in 1763
* **Linear Regression** - formalized by Marie Legendre in 1805
* **Discriminant Analysis** - develpoed by Ronald Fisher in his 1939 paper "The Use of Multiple Measurements in Taxonomic Problems"
* **Monte Carlo Simulation** - pioneered by Stanislaw Ulam and John von Neumann in the early 1940's as part of the Manhattan Project

Upon reflection, one could ask, why didn't the fourth paradigm start before the 1940's and even in the 1800s? What changed? The answer is that other critical developments were made available.

##### Cheap and Available Compute

Consider the following developments in computers.

* **Charles Babbage's Analytical Engine** (1837) is often credited as the first computer, yet is was a mechanical device the attempted to impliment many modern concepts such as arithmetic logic unity, control flow and memory, but it was never completed.

* **Konrad Zuse's Z3** (1941) and **ENIAC** (1945) - first digital, programable computers, but they were programmed by labor-intensive and time-consuming rewiring of plugboards with machine language as there was no high level programming language, the memory could fit 1,000 words limiting the program complexity and with 1000s of vacuum tubes cooling and maintenance was a big challenge. These unreliable machines were very slow with only 5,000 additions per second.

* **Transitors** - invented in 1947 the transitor replaced the vacuum tubes greatly improving energy-efficiency, miniturization, speed and reliability. Resulting in the second generation computers such as **IBM 7090** and **UNIVAC 1108**. 

* **Integrated Circuits** - developed in the 1960s allowed for multiple transitors to be placed on a single chip leading to third generation computers.

* **Microprocessors** - developed in 1971 integrated the functions of a computer's centeral processing unit (CPU) enabling smallers, cheaper computers, resulting in the personal, home computate revolution including the **Apple II** (1977) and **IBM PC** (1981). Yes, when I was in grade 1 in elementary we had a Apple II in my classroom, and it amazed all of us with the monochrome (orange and black pixels) monitor, floppy disk loaded programs (there was no hard drive) and beeps and clicks from the speaker! 

We live in a society with more compute power in our pockets (cell phones) than used to send the first astronaughts to the moon and a SETI screen saver that uses home computers' idle time to search for extraterestrial life! We are no surrounded by cheap and reliable compute that our grandparents (and perhaps parents) could never have imagined. 

As you will learn in this e-book, Machine Learning is a lot of compute. In fact, once we exceed ridge regression training the methods all rely on a large number of iterations and tuning the models required a lot of trained models. Cheap and available compute is an essential prerequisite for the fourth paradigm. Now consider the development of data science has been largely a croud sourced, open source effort. There cannot be data science without everyone having access to efficient compute.

##### Big Data

Parrallel to cheap and accessible compute is the issue of available big data. With small data we tend to rely on other sources of information such as physics, engineering and geoscience principals and then callibrate these models to the few available observations, second and third paradigm methods for scientific discovery. With big data we can learn the full range of behavoirs from the data itself. In fact, with big data we often see the limitations of the second and third paradigm models due to system complexity. 


```{figure} /_static/concepts/ML_workflow.png
```

Therefore, big data:

* precludes exclusive use of the second and thrid paradign methods.
*
* enables 
