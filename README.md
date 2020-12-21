# Welcome to Heatmap Workshop!🤗



# Index
* Introduction

* Steps  
  * Step Zero :  Importing libraries
  * Step One  :  Plotting Scatterplot
  * Step Two  :  Relp Plot
  * Step Three:  Violen plot
  * Step Four :  Pair Grid
  * Step Five :  Heatmap
  
* Application

* Resources for datasets

* Keep Hacking
        * Boxen
        * Heatmap "Cereals"
        * Multivariate Distribution



# INTRODUCTION 

In this workshop you will use python language and its libraries to create stunning heatmap from scratch. Even if you don't know the python language no worries this tutorial  will guide you and keep you intrested. Most importantly you will learn about  heatmap. what is heatmap? and how tp make one like data scientist do!🤗.
Even you can visualize the data, your own data too!


**I m showing you what you will learned after completing  the workshop**

![](https://cloud-fgw5w2l4l.vercel.app/0screenshot_2020-12-20_at_21.41.42.png)

[Click Here to See Working DEMO on Repl](https://repl.it/@ShiveshSingh/Heatmap#main.py)


# Getting started

You just need to setup an account on repl.
Or You can run this program on your Python idle like pycharm, atom, Jupyter notebook and visual studio e.t.c



**Step zero**


**Importing libraries**

**Repl** - when we programming  in repl it automatically imports the libraries and dependencies  with simple command shown below and hit run.
we have used pd as initial  because  we don't have to write whole panda again and again...

``` import pandas as pd ```

        
***YAY! you have completed the first step by importing pandas library*** 

**Now import all libraries 

For you will see [Repl]()
 
For terminal idle based like pycharm, jupyter, atom and visual studio ...
First, You have to go to command line then use this command " Pip install pandas numpy scipy statsmodel matplotlib seaborn "
Above commond line will install all libraries in your idle...

After, You will see this [Command Terminal]() 

As you can see you have successfully  installed all libraries and it's dependencies.

Hip Hip Hooray!

>**One step at a time is all it takes to get you there.
                                                     by Emily Dickinson
                                       
    
    
    
 victory g.i.f


# Know more about the libraries you will going to use :-

## Pandas🐼
pandas (all lowercase) is a popular Python-based data analysis toolkit which can be imported using import pandas as pd. It presents a diverse range of utilities, ranging from parsing multiple file formats to converting an entire data table into a NumPy matrix array. This makes pandas a trusted ally in data science and machine learning.

*pandas

## Numpy🔢
NumPy is a library used for working with arrays. It also has functions for working in domain of linear algebra, fourier transform, and matrices.
Basically it is used to perform large set of mathematical operations on array. array, is a data structure consisting of a collection of elements, each identified by at least one array index or key.

*Array image



## Scipy👨🏻‍🔬
SciPy is an open-source Python library which is used to solve scientific and mathematical problems. It is built on the NumPy extension and allows the user to manipulate and visualize data with a wide range of high-level commands.

* scipy image

## Statsmodel🧮
Statsmodels is a Python package that allows users to explore data, estimate statistical models, and perform statistical tests. An extensive list of descriptive statistics, statistical tests, plotting functions, and result statistics are available for different types of data and each estimator.

*statsmodel image

## Matplotlib📊
A picture is worth a thousand words, and with Python’s matplotlib library, it fortunately takes far less than a thousand words of code to create a production-quality graphic.

*matplotlib img

## Seaborn䷀
Seaborn library is one of the rarest earth metal. If you are science student you will get...😄. Let's talk about seaborn library which is made up in top of the
Matplotlib  library. Matplotlib is mainly deployed for basic plotting. Visualization using Matplotlib generally consists of bars, pies, lines, scatter plots and  so on.

Seaborn: Seaborn, on the other hand, provides a variety of visualization patterns. It uses fewer syntax and has easily interesting default themes.G
Great Right!😲
 
 
 
# Step 1.Plotting Scatter PLot

        import seaborn as sns
        import matplotlib.pyplot as plt


        height = [62, 64, 69, 75, 66, 68, 65, 71, 76, 73]
        weight = [120, 136, 148, 175, 137, 165, 154, 172, 200, 187]

        sns.scatterplot(x=height, y=weight)
        plt.show()
        
 **Output**
        ![]()


# Step 2. Relp plot
        
        import numpy as np
        import pandas as pd
        import matplotlib.pyplot as plt
        import seaborn as sns

        a = sns.load_dataset("flights")
        sns.relplot(x="passengers", y="month", hue="year", data=a)
        plt.show()
        
 **Output**
 ![]()

# Step 3. Violen Plot
        
        import matplotlib.pyplot as plt
        import seaborn as sns

        tips = sns.load_dataset("tips")
        sns.catplot(x="day", y="total_bill", kind="violin", data=tips)
        plt.show()
**Output**
![]()
        
        
# Step 4. Pair Grid
        
        import numpy as np
        import pandas as pd
        import matplotlib.pyplot as plt
        import seaborn as sns
        from scipy import stats


        a = sns.load_dataset("flights")
        b = sns.PairGrid(a)
        b.map(plt.scatter)
        plt.show()
**Output**
![]()


# Step 5. Heat Map
        
        import matplotlib.pyplot as plt
        import seaborn as sns

        flights = sns.load_dataset("flights")
        flights = flights.pivot("month", "year", "passengers")
        ax = sns.heatmap(flights, annot=True, fmt="d", linewidths=5, cmap="YlGnBu")
        
 **Output**
 ![]()






with elpanation


make changes with grammerly :)



complex graph 
with explanaation of only added elememts


what doe this graphs says



#Hacking

one more resources what you can do this Heatmaps

