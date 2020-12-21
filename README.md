**“Creativity is the goal. Coding is just to allow that. Creativity is in the front seat; technology is in the backseat. It is sort of the blend with both of these that you can do such powerful things now.”**
 
# Welcome to Heatmap Workshop!🤗

# Index
* Introduction

* Steps  
  * Step Zero:  Importing libraries
  * Step One:  Plotting Scatterplot
  * Step Two:  Relp Plot
  * Step Three:  Violin plot
  * Step Four:  Pair Grid
  * Step Five:  Heatmap
  
* Application

* Resources for datasets

* Hacking
  * Boxen
  * Heatmap "Cereals"
  * Multivariate Distribution



# INTRODUCTION 

In this workshop, you will use python language and its libraries to create a stunning heatmap from scratch. Even if you don't know the python language no worries this tutorial will guide you and keep you interested. Most importantly you will learn about heatmap. what is a heatmap? and how to make one like data scientists do!🤗.
Even you can visualize the data, your own data too!


**I m showing you what you will learn after completing  the workshop**

![](https://cloud-fgw5w2l4l.vercel.app/0screenshot_2020-12-20_at_21.41.42.png)

[Click Here to See Working DEMO on Repl](https://repl.it/@ShiveshSingh/Heatmap#main.py)


# Getting started

You just need to set up an account on repl Or You can run this program on your Python idle like pycharm, atom, Jupyter notebook, and visual studio e.t.c. Some basic knowledge is required for the computer and you are ready to go!.
I have designed this workshop sweet and simple for you! It just takes 15-20minutes to complete the workshop...
Ready!
get set!
Go!

>**One step at a time is all it takes to get you there.
                                                     by Emily Dickinson
                                       

## Step zero

### This is for repl users.
 **Importing libraries**

### Repl - when we program in repl it automatically imports the libraries and dependencies with the simple command shown below and hit run.
we have to use pd as initials because we don't have to write the whole panda again and again...

``` import pandas as pd ``` 

       
***YAY! you have completed the first step by importing pandas library*** 




### This is for idle users

 **Now importing  all libraries for idles

For terminal idle based like pycharm, Jupiter, atom and visual studio ...
First, You have to go to the command line then use this command 
   
  ``` pip install pandas numpy scipy statsmodel matplotlib seaborn ```
   
The above command line will install all libraries in your idle...

After, You will see this [Command Terminal]() 

As you can see you have successfully installed all libraries and their dependencies.

Hip Hip Hooray!

the last step and set up is done download [Dataset file]()
add this in your project folder.
    
    
    
 victory g.i.f


# Know more about the libraries you will going to use:-
 ![](library_collage_img)

## Pandas🐼
pandas is a popular Python-based data analysis toolkit that can be imported using import pandas as pd. It presents a diverse range of utilities, ranging from parsing multiple file-formats to converting an entire data table into a NumPy matrix array. This makes pandas a trusted ally in data science and machine learning.

## Numpy🔢
NumPy is a library used for working with arrays. Basically, it is used to perform a large set of mathematical operations on an array. An array is a data structure consisting of a collection of elements, each identified by at least one array index or key.

## Scipy👨🏻‍🔬
SciPy is an open-source Python library that is used to solve scientific and mathematical problems. It is built on the NumPy extension and allows the user to manipulate and visualize data with a wide range of high-level commands.

## Statsmodel🧮
Statsmodels is a Python package that allows users to explore data, estimate statistical models, and perform statistical tests. An extensive list of descriptive statistics, statistical tests, plotting functions, and result statistics are available for different types of data and each estimator.

## Matplotlib📊
A picture is worth a thousand words, and with Python’s matplotlib library, fortunately, takes far less than a thousand words of code to create a production-quality graphic.

## Seaborn䷀
Seaborn library is one of the rarest earth metals. If you are a science student you will get...😄. Let's talk about the seaborn library which is made up on top of the
Matplotlib library. Seaborn: Seaborn, on the other hand, provides a variety of visualization patterns. It uses fewer syntax and has easily interesting default themes.
Great Right!😲
 
 
 
# Step 1.Plotting Scatter PLot

        import seaborn as sns
        import matplotlib. pyplot as plt

**Adding variable height and weight to store the values to be plotted. we have used list data-type to store these values in height and weight.

        height = [62, 64, 69, 75, 66, 68, 65, 71, 76, 73]
        weight = [120, 136, 148, 175, 137, 165, 154, 172, 200, 187]
        
**Here sns as a reference seaborn library
**And we are also using plot type: scatterplot 

        sns.scatterplot(x=height, y=weight)
**plt.show is used to display the plot on your display
        
        plt.show()
        
 **Output**
        ![]()


# Step 2. Relp plot
        
        import numpy as np
        import pandas as pd
        import matplotlib.pyplot as plt
        import seaborn as sns

**Initializing a variable to load the datasets in variable named flights
       
       flights = sns.load_dataset("flights")
       
**sns is referring to the seaborn library
**plot type: relplot

       sns.relplot(x="passengers", y="month", hue="year", data=flights)
**plt.show is used to display the plot on your display
      
       plt.show()
        
 **Output**
 ![]()
 
 **Data-set required named "flights"

# Step 3. Violin Plot
        
        import matplotlib.pyplot as plt
        import seaborn as sns
**Loading "tips" data set in tips variable

        tips = sns.load_dataset("tips")
**Plot type: catplot kind: violin

        sns.catplot(x="day", y="total_bill", kind="violin", data=tips)
        plt.show()
**Output**
![]()

**Data-set required named "tips"
        
        
# Step 4. Pair Grid
        
        import numpy as np
        import pandas as pd
        import matplotlib.pyplot as plt
        import seaborn as sns
        from scipy import stats


        a = sns.load_dataset("flights")
        
**Grape type: PairGrid we have used this as variable

        b = sns.PairGrid(a)
        
        b.map(plt.scatter)
        
**Visualising type: scatter
        
        plt.show()
       
**Output**
![]()

**Data-set required "flights"


# Step 5. Heat Map
        
        import matplotlib.pyplot as plt
        import seaborn as sns

        flights = sns.load_dataset("flights")
        
**pivot is used so we can handle duplicate values for one index/column pair

        flights = flights.pivot("month", "year", "passengers")
        
**annot: the value will show on each cell of the heatmap
**fmt: adding annotations.
***linewidth: width between each box
***cmap: cmap is a color template that we have used.

        ax = sns.heatmap(flights, annot=True, fmt="d", linewidths=5, cmap="YlGnBu")
        
 **Output**
 ![]()

**Data-set required "flights"


# voilà! 
>**congratulations  you have completed the workshop**


# Keep Hacking!
**You can create a lot of variety of heatmap as I have created below 
You can try these, If you want to learn more
