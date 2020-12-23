---
name: Heatmap
description: Data visualisation with Seaborn
author: shivesh01
---

**“Creativity is the goal. Coding is just to allow that. Creativity is in the front seat; technology is in the backseat. It is sort of the blend with both of these that you can do such powerful things now.”**                                             by       Tim cook
 
# Welcome to Heatmap Workshop!🤗
![Slideshow](https://cloud-49dp118l9.vercel.app/0slidshow.gif)

[Click Here to See Working HEATMAP DEMO on Repl](https://repl.it/@ShiveshSingh/Heatmap#main.py)

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


# INTRODUCTION 

In this workshop, you will be using python language and its libraries to create a stunning heatmap from scratch. Even if you don't know the python language no worries this tutorial will guide you and keep you interested. Most importantly you will learn about heatmap. let's talk about what is a heatmap? and how to make one like data scientists do!🤗.
A heat map (or heatmap) is a graphical representation of data where values are depicted by color. Heat maps make it easy to visualize complex data and understand it at a glance:
Even you can visualize the data, your own data too!

--
> One step at a time is all it takes to get you there.
                                                     by Emily Dickinson
--                                                 


# Getting started

You just need to set up an account on repl or you can run this program on your Python idle like pycharm, atom, Jupyter notebook, and visual studio e.t.c. Some basic knowledge is required for the programming and you are ready to go!.
I have designed this workshop sweet and simple for you! It just takes 15-20minutes to complete the workshop...
Ready!
get set!
Go!
                                       

## Step zero!

### Setting up an account on repl

- Go to the repl website and sign up 
[Repl website](https://repl.it/signup) and create a file


![repl website](https://cloud-5pg8raikb.vercel.app/0screenshot_2020-12-23_at_10.38.39.png)   ![create file](https://cloud-5pg8raikb.vercel.app/1screenshot_2020-12-23_at_11.13.43.png)

- create a file  by clicking **+ New repl** and choose programming language **python** and named it as you want and click **create repl**

- Download the datasets from a simple click and Drag and drop to the folder in which you are working on repl.
 ---         --- 
**Data-sets** [flights](https://cloud-5jao3dtbu.vercel.app/0flights.csv "click to download") and [tips](https://cloud-1oaqj43if.vercel.app/0tips.csv "click to download") 
 ---         ---

- Rename these file as flights and tips in repl folder in which you are working

- you are ready to code!


# You have done a fantastic work by completing step zero!👏

**Advantage of working on repl**

*when we program in repl it automatically imports the libraries and dependencies with the simple command. So, You just need a replt account or any python idle to get started*
     
# Know more about the libraries you will going to use:

## Pandas🐼
Pandas is a popular Python-based toolkit. It presents a diverse range of utilities like converting an entire data table into a NumPy matrix array and much more. This makes pandas a trusted ally in data science and machine learning.

## Numpy🔢
NumPy is a library used for working with arrays. Basically, it is used to perform a large set of mathematical operations on an array. An array is a data structure consisting of a collection of elements, each identified by at least one array index or key.

## Scipy👨🏻‍🔬
SciPy is an open-source Python library that is used to solve scientific and mathematical problems. It is built on the NumPy extension and allows the user to manipulate and visualize data with a wide range of high-level commands.

## Statsmodel🧮
Statsmodels is a Python package that allows users to explore data, estimate statistical models, and perform statistical tests.

## Matplotlib📊
A picture is worth a thousand words, and with Python’s matplotlib library, fortunately, takes far less than a thousand words of code to create a production-quality graphic.

## Seaborn䷀
Seaborn library is one of the rarest earth metals. If you are a science student you will get...😄. Seaborn, provides a variety of visualization patterns. It uses fewer syntax and has interesting default themes.
Great Right!😲
 
 # Step 1.Plotting Scatter PLot
```python 

        import seaborn as sns
        import matplotlib. pyplot as plt

# Adding variable height and weight to store the values to be plotted. we have used list data-type to store these values in height and weight.

        height = [62, 64, 69, 75, 66, 68, 65, 71, 76, 73]
        weight = [120, 136, 148, 175, 137, 165, 154, 172, 200, 187]
        
# Here sns as a reference seaborn library
# And we are also using plot type: scatterplot 

        sns.scatterplot(x=height, y=weight)
# plt.show is used to display the plot on your display
        
        plt.show()
```
        
 **Output**
 
 ![Scatter plot](https://cloud-ikhasazgz.vercel.app/3scatter_plot.png )


# Step 2. Relp Plot
        
```python
        import numpy as np
        import pandas as pd
        import matplotlib.pyplot as plt
        import seaborn as sns

# Initializing a variable to load the datasets in variable named flights
       
       flights = sns.load_dataset("flights")
       
# sns is referring to the seaborn library
# plot type: relplot

       sns.relplot(x="passengers", y="month", hue="year", data=flights)
       
# plt.show is used to display the plot on your display
      
       plt.show() 
```
        
 **Output**
 
 ![Relp plot](https://cloud-ikhasazgz.vercel.app/2relp_plot.png)
 
 **Data-set required named [flights](https://cloud-5jao3dtbu.vercel.app/0flights.csv "click to download")

# Step 3. Violin Plot
```python        
        import matplotlib.pyplot as plt
        import seaborn as sns
# Loading "tips" data set in tips variable

        tips = sns.load_dataset("tips")
# Plot type: catplot kind: violin

        sns.catplot(x="day", y="total_bill", kind="violin", data=tips)
        plt.show()
```

**Output**

![Violen plot](https://cloud-ikhasazgz.vercel.app/4violin_plot.png)

**Data-set required named [tips](https://cloud-1oaqj43if.vercel.app/0tips.csv "click to download")
        
        
# Step 4. Pair Grid
```python     
        import numpy as np
        import pandas as pd
        import matplotlib.pyplot as plt
        import seaborn as sns
        from scipy import stats


        a = sns.load_dataset("flights")
        
# Grape type: PairGrid we have used this as variable

        b = sns.PairGrid(a)
        
        b.map(plt.scatter)
        
# Visualising type: scatter
        
        plt.show()
```
        
       
**Output**

![Pair Grid](https://cloud-ikhasazgz.vercel.app/1pairgrid.png)

**Data-set required [flights](https://cloud-5jao3dtbu.vercel.app/0flights.csv "click to download")

# Step 5. Heat Map
        
```python
        import numpy as np
        import matplotlib.pyplot as plt
        import seaborn as sns

        flights = sns.load_dataset("flights")
        
# pivot is used so we can handle duplicate values for one index/column pair

        flights = flights.pivot("month", "year", "passengers")
        
# annot: the value will show on each cell of the heatmap
# fmt: adding annotations.
# linewidth: width between each box
# cmap: cmap is a color template that we have used.

        ax = sns.heatmap(flights, annot=True, fmt="d", linewidths=5, cmap="YlGnBu")
```
        
 **Output**
 ![Heatmap](https://cloud-ikhasazgz.vercel.app/0heatmap.png)

**Data-set required [flights](https://cloud-5jao3dtbu.vercel.app/0flights.csv "click to download")


# voilà!

**congratulations!✌️  you have completed the workshop. Share with your friends and family.
Frankly share with everyone🤗✌️🥳👏🏅🌇🎊

![congratulations  g.i.f](https://cloud-mga2rf9gs.vercel.app/4tenor__1_.gif)

### You can create a lot of variety of heatmap as I have created below
 ![flight heatmap](https://cloud-tgw4nss32.vercel.app/0heatmap_2.png)


```python

import matplotlib.pyplot as plt
import seaborn as sns
import numpy as np

flights = sns.load_dataset("flights")
flights = flights.pivot("month", "year", "passengers")
corr = np.corrcoef(np.random.randn(10, 200))
mask = np.zeros_like(corr)
mask[np.triu_indices_from(mask)] = True
with sns.axes_style("white"):
    f, ax = plt.subplots(figsize=(7, 5))
    ax = sns.heatmap(corr, mask=mask, vmax=.3, square=True)
plt.show()
```

![flight heatmap staircase](https://cloud-tgw4nss32.vercel.app/1heatmap_4.png)
  **Data-set required named [flights](https://cloud-5jao3dtbu.vercel.app/0flights.csv "click to download")


```python
import matplotlib.pyplot as plt
import seaborn as sns
import numpy as np

flights = sns.load_dataset("flights")
flights = flights.pivot("month", "year", "passengers")
grid_kws = {"height_ratios": (.9, .05), "hspace": .3}
f, (ax, cbar_ax) = plt.subplots(2, gridspec_kw=grid_kws)
ax = sns.heatmap(flights, ax=ax,
                 cbar_ax=cbar_ax,
                 cbar_kws={"orientation": "horizontal"})
plt.show()
```
 **Data-set required named [flights](https://cloud-5jao3dtbu.vercel.app/0flights.csv "click to download")


# Keep Hacking!

You can learn these graph plots too!

![](https://cloud-8c3mmthaa.vercel.app/0keep_hacking.png "You can make it happen!")
Resources

- [Univariate Distribution of Birth Rate](https://towardsdatascience.com/visualize-world-trends-using-seaborn-in-python-2e563e7d35da)
- [Cat plot Life Expectancy of people in different of the world](https://cmdlinetips.com/2019/03/catplot-in-seaborn-python/)
- [Cereals compositions Heatmap](https://towardsdatascience.com/heatmap-basics-with-pythons-seaborn-fb92ea280a6c)


