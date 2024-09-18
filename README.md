# Movify - Movie Recommendation System
## Submission for Finals Project '24


<p align="center">
  <img src="https://github.com/user-attachments/assets/ada6c7dc-29ad-4ffa-94cd-9b786c8c462a" alt="Movify image" width="50%" />
</p>


## Overview
Movify is a movie recommendation system that offers generalized recommendations to every user based on movie popularity, genre, and year. 
The model also gives personalized recommendations based on the user's choice of genre and cast.
Finally, the system suggests similar movies have a higher probability of being liked based on the movie selected by the user. 


## Demo Video
The demo video for the app can be checked here: [Movify | Video]()


## Features
1. Sign-up and Sign-in functionality. ✔️

2. Forgot password (resetting password) functionality. ✔️

3. OTP validation. ✔️

   `The user receives a mail containing OTP for validation before resetting the password.`

4. Restrictions and validations on the sign-up page, sign-in page, forgot password functionality, OTP validation page, and reset password page. ✔️
   
5. The User’s credentials are stored in the database. ✔️
  
6. Completely responsive front end. ✔️

7. A total of 4 types of recommendations:
  * Recommended movies based on the user's chosen genres and casts. ✔️
  * Most popular movies based on different genres. ✔️
  * Most popular movies based on different years. ✔️
  * Recommended movies similar to the user's selected movie. ✔️
  
8. Movie details and trailer linked for each movie. ✔️

9. Watch a movie option. ✔️

10. Option to like or dislike a movie. ✔️

11. Client-side session tracking. ✔️

12. Continuous deployment. ✔️


## Interfaces

### Landing Page
* Seamless landing page with `Sign-in` and `Sign-up` (Get Started) button.

![home page](https://github.com/user-attachments/assets/092ecc54-f128-4c0e-8eaf-e99aaaa0a763)

### Sign-up Page

![sign-up page](https://github.com/user-attachments/assets/edc77e99-9ad0-4b07-9b33-340eb50187d6)

### Sign-in Page

![5 - sign-in](https://github.com/user-attachments/assets/e9b1a475-3cb4-4fb9-aa69-09f48da8785e)

### OTP Validation Page

![11 - otp validation](https://github.com/user-attachments/assets/4c737298-0c95-4e3c-bea4-428bd801075c)

### Reset password Page

![14 - reset](https://github.com/user-attachments/assets/e9b1a475-3cb4-4fb9-aa69-09f48da8785e)

### Restrictions and validations on the sign-up page, sign-in page, forgot password functionality, OTP validation page, and reset password page
* All fields not filled
* Email account already registered (sign-up), Email account not registered (sign-in)
* Incorrect password, OTP incorrect
* Email address not entered, OTP not entered, new password not entered

![6 - validations](https://github.com/user-attachments/assets/cae4b0dc-3f75-4d8f-8cda-b3db2b133664)

### Choices Page
* Page for choosing preferred genres and casts used for recommending movies

![choices](https://github.com/user-attachments/assets/0b8bf436-d712-407c-b3cf-8a007e4a8b29)

### Recommendations page
* This page shows recommended movies based on genres and casts chosen by the user.
* It also displays the most popular movies based on different genres and years.

![16 - recommendations](https://github.com/user-attachments/assets/c1e4006f-2256-4685-969c-993ed0579c00)

### Movie Page
* This page shows details and a trailer of the movie selected by the user.
* It also recommends similar movies to the user based on the selected movie.

![18 - movie](https://github.com/user-attachments/assets/6bc34d43-a3e1-4232-a902-187b49148737)

### Watch Movie Page
* This page is to watch the movie selected.

![19 - watch](https://github.com/user-attachments/assets/4d5cfd32-2345-48c6-b8be-f8cc500fb9cd)


## Tech Stack and Software used
1. `Frontend`: HTML5, CSS3, JavaScript, BootStrap, jQuery
2. `Backend`: Python flask
3. `Database`: PostgreSQL, SQLite3
4. `ML model`: Jupyter Notebook
5. `IDE`: PyCharm
6. `Version Control`: Git
7. `Deployment`: Heroku

You can also see the list of dependencies in the [requirements.txt](/requirements.txt) file.


## Libraries and Toolkits used
`Python`: NumPy, Pandas, ast (Abstract Syntax Trees), pickle

`ML`: ntlk (Natural Language Toolkit), sklearn (scikit-learn)

`SQLite`: sqlite3, SQLAlchemy


## Recommendation Algorithm
For recommendations of similar movies, a content-based recommendation system. For recommendation, the system takes into account movie titles, genres, starring cast, keywords, overview, and the director. I have implemented the Cosine Algorithm after the vectorization of movies. 
It is achieved by using the Annoy (Approximate Nearest Neighbors) mechanism. Resource for Annoy: https://github.com/spotify/annoy


## Deployment
For Deployment, I have used `Heroku` as a platform.
A deployed version can be checked here: [Movify]()


## Installation/Environment Setup
1. Clone this repository in your local system.
* Open the terminal in a new folder and enter the command given below.
   <!-- ```
   git clone https://github.com/DEV7879/Movify.git
   ``` -->
   ```
   git clone https://github.com/DEV7879/Movify.git
   ```

2. Make sure that Python is installed and updated in your machine.

3. Install dependencies.
* Open the terminal in the cloned folder and enter the command given below.
   ```
   pip3 install -r requirements.txt
   ```
  
4. Run the project.
* While you are still inside the cloned folder, write the following command in the terminal to run the website locally. 
   ```
   python app.py
   ```
   
5. If everything is done in order, the app will be running at "http://127.0.0.1:5000"


## CD Setup
For continuous deployment, Heroku is used. Any changes pushed to the main branch will be automatically deployed. 


## Future Scope
* `Like/Dislike`: The option to like or dislike a movie adds the movie to the user's like/dislike list. As of now, I am just accumulating the data. This can be further extended by using the like/dislike list to recommend movies to the user.

* `Watch Movie`: The watch movie option currently displays the same movie intro for all the movies. In the future, it can be customized according to the movie selected.

* `Collaborative Filtering`: The model currently uses a content-based recommendation system. It can be converted into a hybrid system by adding a collaborative filtering mechanism.


## Documentation
A complete project report for the system with a use case diagram, web flow, ER diagram, wireframes, etc can be found here: [Movify | Project Report](/documents/ProjectReport.docx.pdf).

A short and crisp version of the documentation can be found here: [Movify | Documentation](/documents/Documentation.pdf).

A presentation for the project can be found here: [Movify | Presentation](/documents/Presentation.pdf).


<br><hr>
Thank you ❤️
