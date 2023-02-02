# ACM 2023 Spring Coding Challenge
## Introduction
This was my first experience with a coding challenge of this type, where the problem was more similar to data science and dealt with csv files.
As such, I was exposed to a lot of new technologies, such as the pandas, matplotlib, and scikit-learn libraries for python.

## Problem
I wasn't really sure what to do with the data set since I'm not very familiar with astrophysics or how stars work, so I decided to just see how many of the sample problems on the main github repo that I could do.
1. Finding the most common star in the data
This was pretty simple, but I still learned a lot about pandas and matplotlib in the process of learning for later problems.
My solution was to plot a histogram of the 'Star type' column of the csv when converted to a pandas dataframe. which is shown below
![image](https://i.imgur.com/mRXltm3.png)

2. Finding correlations in the data

This was pretty much identical with the first problem, only difference being that instead of plotting a histogram of one variable, I plotted a scatter plot against two variables.
3. Finding which properties are most influential in classifying a star's type
After looking at the graphs, I saw that Absolute magnitude, luminosity, and radius were the most influential
![image](https://i.imgur.com/fglRArI.png)
4. Creating a Hertzsprung-Russel diagram
This was essentially a scatterplot plotting absolute magnitude vs temperature, except I had to map each Star color value with a hex value and use that in the scatterplot generation
![image](https://i.imgur.com/LejGf5A.png)
5. Using a machine learning model to predict the star type of a row of data
This was the hardest/most time consuming part of the challenge. I decided to use scikit-learn, but in the future I'd like to learn how to use PyTorch or TensorFlow as well.
A challenge I ran into was that star color and spectral class were qualitative variables, so I had to learn how to use sklearn's column transformer along with the OneHotEncoder in order to turn those variables into something that the model could understand.
A more detailed writeup is available in the .ipynb file.
