# Exploratory Data Analysis of Medium articles dataset
The dataset contains 6000+ articles published in 2019 from the following 7 different publications:
* The Startup
* Towards Data Science
* Data Driven Investor 
* UX Collective 
* The Writing Cooperative
* Better Marketing 
* Better Humans

The dataset can be found [here](https://www.kaggle.com/datasets/dorianlazar/medium-articles-dataset?select=medium_data.csv) 

The following exploratory analysis were carried out:
- Assessing the Data
- Cleaning
- Exploratory Visualization

## Assessing Data
The dataset contains 6508 article enteries and 10 columns. Only the subtitle and image columns have null values. The subtitle column has 46.54% missing data while image column has 2.26% missing values

## Cleaning
On a closer inspection of the data, the responses column contained some string inputs making the column an object datatype. The affected rows were dropped and the datatype converted to integer
The image type of the images uploaded were attached to numbers. The image type was extracted into a column called image_type.
For the image_type column, uppercase and lowercase of same image type were recognized differently so the column was converted to lowercase. Jpeg and Jpg refer to thesame type of image so all instances of jpeg were converted to jpg.

## Exploratory Visualization
jpg images were the commonest image type
About 45% of the publication on Medium in 2019 were The Startup articles.
Although The startup publication has the highest number of publication and highest number of responses put together, they do not have the highest average response per article. Instead Better Humans and Better Marketing articles have the highest number of responses per article published.
There seems to be a linear correlation between number of responses and claps.
