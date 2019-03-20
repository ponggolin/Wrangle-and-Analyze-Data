# Wrangle and Analyze Data
Real-world data rarely comes clean. Using Python and its libraries, I will gather data from a variety of sources and in a variety of formats, assess its quality and tidiness, then clean it. This is called data wrangling. I will document the wrangling efforts in a Jupyter Notebook, plus showcase them through analyses and visualizations using Python (and its libraries) and/or SQL.

## What Software Do I Need?

The following packages (i.e. libraries) need to be installed.

- pandas
- numpy
- requests
- tweepy
- json

# The Data

### Enhanced Twitter Archive

The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced."

### Additional Data via the Twitter API

Back to the basic-ness of Twitter archives: retweet count and favorite count are two of the notable column omissions. Fortunately, this additional data can be gathered by anyone from Twitter's API. Well, "anyone" who has access to data for the 3000 most recent tweets, at least. But we, because we have the WeRateDogs Twitter archive and specifically the tweet IDs within it, can gather this data for all 5000+. And guess what? We're going to query Twitter's API to gather this valuable data.

### Image Predictions File

One more cool thing: I ran every image in the WeRateDogs Twitter archive through a neural network that can classify breeds of dogs*. The results: a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images).

## Project Details

We will perform the following tasks in this project:

Data wrangling, which consists of:

- Gathering data
- Assessing data
- Cleaning data

Storing, analyzing, and visualizing our wrangled data

Reporting on 1) data wrangling efforts and 2) data analyses and visualizations.

## Resource
https://github.com/abodacs/Wrangle-and-Analyze-Data-DAND-project
https://github.com/RedRock42/Udacity-Nanodegree-Portfolio/tree/master/P4.Wrangling%20%26%20Analyzing%20Twitter%20Data
https://github.com/MrGeislinger/UdacityDAND_Proj_WrangleAndAnalyzeData
https://github.com/gouravaich/data-analyst-nanodegree/tree/master/P3%20-%20Wrangle%20and%20Analyze%20Data
https://stackoverflow.com/questions/42518864/convert-json-data-from-request-into-pandas-dataframe
https://anaconda.org/conda-forge/tweepy
https://stackoverflow.com/questions/16419670/increase-distance-between-title-and-plot-in-matplolib
https://stackabuse.com/reading-and-writing-json-to-a-file-in-python/