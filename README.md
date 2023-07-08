# FlickFlow-Movie-Recommendation-System

The following stacks were used
![Python](https://img.shields.io/badge/Python-3.9-blueviolet)
![Framework](https://img.shields.io/badge/Framework-Flask-red)
![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-green)
![API](https://img.shields.io/badge/API-TMDB-fcba03)

This application provides all the details of the requested movie such as overview, genre, release date, rating, runtime, top cast, reviews and recommended movies.

The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, web scraping has been performed to get the reviews given by the user in the IMDB site using `beautifulsoup4` and sentiment analysis has been performed on these reviews.

## Note
If you can't find the movie you're searching for through auto-suggestions while typing, there's no need to worry. Simply type the name of the movie and press "enter". Even if you make some typos, it should still work fine.


## The API key

Create an account on https://www.themoviedb.org/, click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your `API` sidebar once your request is approved.

## How to run the project?

1. Clone this repository in your local system.
2. Train and save `.pkl` files for predicting if the Movie reviews are good or bad. 
3. Install all the libraries mentioned in the `requirements.txt` file with the command `pip install -r requirements.txt`.
4. Replace YOUR_API_KEY at line no. 2 of `static/recommend.js` file.
5. Open your terminal/command prompt from your project directory and run the `main.py` file by executing the command `python main.py`.
6. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
7. Hurray! That's it.

## Architecture
The following image shows the workflow of the app "FlickFlow:  Navigate the World of Movies"
![Recommendation app]()

### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)


