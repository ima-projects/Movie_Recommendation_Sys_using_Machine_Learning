# Movie Recommendation System using Machine Learning

Building a content and popularity-based movie recomendation system in Python where a user can provide a name of their favourite movie and the recommendation system will generate a list of movies based on their input. This is similar to popular streaming recommendation systems used by Netflix and Prime Video. 

## Table of Contents
- [Business Problem](#business-problem)
  * [Objective](#objective)
  * [Goal](#goal)
- [Data Source](#data-source)
- [Methods](#methods)
- [Tech Stack](#tech-stack)
- [Quick Analysis of Recommender System Results](#quick-analysis-of-recommender-system-results)
  * [Feature Selection and Importance](#feature-selection-and-importance)
  * [Insights and Recommendations Derived from Experimental Analysis](#insights-and-recommendations-derived-from-experimental-analysis)
  * [Limitations and Suggestions for Optimization of the Recommendation System](#limitations-and-suggestions-for-optimization-of-the-recommendation-system)
- [Installation: Simplify Your Analysis](#installation-simplify-your-analysis)
  * [Run in Google Colab](#run-in-google-colab)
  * [Run Locally in Jupyter Notebook](#run-locally-in-jupyter-notebook)




## Business Problem
### Objective:
ABC Streaming Service is a popular platform for streaming movies and TV shows. In order to improve their user experience and increase customer retention, ABC Streaming Service wants to develop a movie recommendation system that helps users discover new movies they will enjoy. However, traditional recommendation systems based solely on user ratings and movie genres are not providing sufficiently personalized recommendations. 

### Goal:
To solve this problem, the goal of this project is to develop a movie recommendation system that incorporates a unique approach to movie analysis, such as using keyword similarity for sentiment analysis of user reviews, in addition to traditional data sources.

The recommendation system will synthesise fundamental principles of data analysis and data science, including:
* How to carry out data collection and pre-processing of various data sources, including user ratings, movie metadata, and other sources of movie information. 
* Create a system using cosine similarity to find movies that are similar to each other based on their features, such as the genre, keywords, tagline, cast and director. 

This will produce results that should be able to provide users with more accurate and diverse recommendations, leading to increased user engagement and satisfaction. This in turn will drive higher retention rates and reduce churn leading to increased revenue for the upcoming quarter.

## Data Source
[Kaggle data source containing movies and tv shows](https://www.kaggle.com/datasets/rachanakoniki/movies)

## Methods
- Exploratory data analysis

## Tech Stack
- Python (in place of a requirement.txt, the four dependencies used are listed in the [Installation](#installation-simplify-your-analysis) section below)
- Google Colab

## Quick Analysis of Recommender System Results
Recommendation list generated after user input of: **iron man**

<img src="./img-movrec.png" alt="movie recs">

### Feature Selection and Importance
- This is a content and popularity-based recommendation system. That is why it will incorporate features such as the movie title, cast, director, genre, description and theme. 
- Textual data, such as words or sentences, cannot be directly processed by most machine learning algorithms, which typically require numerical inputs. Therefore, a process called feature extraction is used to convert the textual data into numerical values that can be used as input to these algorithms. Here the movies are converted into vectors.
- After the user provides the input, the similarity confidence scores are used to generate a list of recommended movies for a user based on their preferences. The Cosine Similarity Algorithm is used to find the similarity between the vectors.
- This results in a list of movies generated that can then be suggested to the user.

### Insights and Recommendations Derived from Experimental Analysis
- Most of the movie suggestions in the data source contain more mainstream recommendations.

### Limitations and Suggestions for Optimization of the Recommendation System
- Can add more movie sources in the future to compare popularity of movie, movie genre, etc. based on location. 
- I can also do this for streaming platforms and provide more granular information on content or popularity of movie(s) based on results of user input and/or location. 

## Installation: Simplify Your Analysis
### Run in Google Colab
1. Open your web browser and go to the Google Colab homepage at https://colab.research.google.com/.
2. Click on "File" > "New notebook" to create a new Colab notebook.
3. In the first cell of the notebook, enter the following code to clone the repository:
```bash
!git clone https://github.com/ima-projects/Movie_Recommendation_Sys_using_Machine_Learning.git
```
4. Run the code cell by clicking on the "Play" button or by pressing "Shift+Enter".
5. Once the repository has been cloned, navigate to the cloned repository folder by entering the following code in a new cell to ensure you are in the correct folder:
```shell
%cd Movie_Recommendation_Sys_using_Machine_Learning/
```
6. Run the code cell by clicking on the "Play" button or by pressing "Shift+Enter".
7. Import dependencies e.g numpy, pandas, difflib and sklearn

8. Run the code cell by clicking on the "Play" button or by pressing "Shift+Enter".

You can now start working with the project in Google Colab. You can open and modify files, run scripts, and execute commands as you would in a local environment.



### Run Locally in Jupyter Notebook
1. Open your web browser and go to the Jupyter website at https://jupyter.org/.
2. Click on "Install" to access the installation instructions for Jupyter notebooks. Follow the instructions for your operating system to install Jupyter on your local machine.
3. Once Jupyter is installed, open a command prompt or terminal and navigate to the directory where you want to store your notebook files.
4. Enter the following command to clone the repository:
```bash
git clone https://github.com/username/Movie_Recommendation_Sys_using_Machine_Learning.git
```
5. Navigate to the cloned repository folder by entering the following command in the command prompt or terminal to ensure you're in the correct folder:
```bash
cd Movie_Recommendation_Sys_using_Machine_Learning/
```
6. Import or install dependencies e.g numpy, pandas, difflib and sklearn

7. Run the Jupyter notebook server by entering the following command in the command prompt or terminal:
```
jupyter notebook
```
This will start the Jupyter notebook server and open a web browser window displaying the Jupyter dashboard.

8. Click on the notebook file you want to run to open it in a new tab in the web browser.
9. In the notebook, you can execute each cell by clicking on it and then clicking on the "Run" button in the toolbar, or by pressing "Shift+Enter".
10. You can modify the notebook code and execute it as you see fit.



