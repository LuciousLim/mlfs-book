# Lab Assignment 1

We aim for grade A in this assignment. And the city we chose is Xiamen, China.

The code is in `./notebooks/airquality`

What we have done:

1. for grade E: we have gone through all the procedures in the notebooks (in `./notebooks/airquality`). And we have implemented all the pipelines as instructed by the notebooks. We also configured the GitHub Action workflow and deployed the dashboard on GitHub Pages ([link](https://luciouslim.github.io/mlfs-book/air-quality)).

2. for grade C: we have added a new feature called `pm25_rolling`, which is the mean value of pm25 of the previous 3 days. And we have put this new feature into all the pipelines. When predicting multiple days ahead we iteratively use predicted pm25 value before to calculate `pm25_rolling`.

3. for grade A: we have refactored the code for all the pipelines to support street-level prediction, where we take into account all the sensors (of the streets) in a city. So now in the dashboard it shows all the sensors of Xiamen, China. (Note: there are only two sensors with pm25 data in this city. But our code can support any city with more sensors as well.)