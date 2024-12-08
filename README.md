# MovieRecommendation_DBMS

### Introduction
In today's world where streaming services offer so many different movies and shows, 
finding the right movie can feel overwhelming. To solve this problem, we recommend 
a movie recommendation system. It's a smart platform designed to make watching 
movies more enjoyable. It provides personalized recommendations based on each 
user's preferences and viewing habits. Our goal is to create a system that understands 
what users like and adapts as their interests change. By analyzing user profiles, 
viewing history, and movie ratings, the system aims to provide tailored 
recommendations that not only save time but also introduce viewers to films they 
might not have otherwise discovered.

## 1. DATABASE PLANNING
### Overview
Several important features have been integrated to improve the functionality of the 
movie recommendation system. It tracks the user's viewing history and preferences, 
making various suggestions that are updated over time. Users can rate the movies they 
watch, which helps improve the accuracy of future recommendations. The system also 
uses advanced methods to create personalized recommendations and allows users to 
browse through different movie categories and genres. The database is organized with 
the necessary tables for user profiles, movie descriptions, ratings, genres, viewing 
history, and recommendations. In the future, we plan to add social features to share 
recommendations, implement real-time updates for more relevant suggestions, and 
include a manual spelling correction feature to improve data accuracy. Overall, this 
project aims to improve the way viewers discover and enjoy movies, making the 
movie viewing experience more engaging and enjoyable.
### Key Features
#### • Track User Watch History and Preferences: 
The system monitors the movies that users have watched and their preferences (e.g., 
favorite genres or actors), enabling more accurate recommendations.
#### • Collect Ratings for Movies:
Users can rate movies on a scale from 1 to 5, which helps to aggregate data on movie 
quality and popularity.
#### • Generate Movie Recommendations:
Utilizing collaborative filtering (which recommends movies based on the preferences 
of similar users)
#### • Option to Browse Movie Categories and Genres:
Users can explore movies by categories and genres, making it easier to discover new 
content that matches their interests.
#### • Social Feature for Users to Share Recommendations:
This feature allows users to connect with friends and share their movie 
recommendations, creating a community feel within the platform.
#### • Real-Time Updates of Recommendations:
The system updates recommendations based on recent user activities, ensuring that 
users always receive relevant suggestions.
#### • Auto Spelling Correction for User-Inputted Data:
An automatic spelling correction feature improves the accuracy of user inputs, 
correcting common spelling errors before the data is stored.

## 2. System Definition

### ➢ Purpose of System: 
This system is designed to help users discover and enjoy movies that match their 
tastes. By keeping track of what users watch, their ratings, and their preferences, the 
system provides personalized movie recommendations. It also allows users to explore 
different genres and share their favorite movies with friends.
### ➢ Scope of System:
The system will include the following features:
#### • User Profiles:
Each user will have a profile that stores their watch history, movie ratings, and 
preferences.
#### • Movie Database:
A comprehensive collection of movies, including details like titles, genres, and user 
ratings.
#### • Recommendation Engine:
A smart system that suggests movies based on what users have watched and rated, 
using advanced methods to ensure accuracy.
#### • Genre Browsing:
users can browse through various movie genres and categories to find films they 
might like.
#### • Social Features:
Users will be able to share their movie recommendations with friends, encouraging 
social interaction.
#### • Real-Time Updates:
The system will provide up-to-date recommendations based on users' recent activities.
#### • Spelling Correction:
Auto spelling correction for user inputs to improve the accuracy of movie searches 
and ratings.

## 3. Requirement Collection and Analysis

### ➢ Fact-Finding Techniques
#### 1. Interviews:
##### • Purpose:
Interviews were held with potential users, including both movie lovers and casual 
viewers. The goal was to understand what they like, the difficulties they face when 
trying to find movies, and the features they want in a recommendation system.
##### • Process:
Structured Interviews: We used a set of specific questions to guide the conversation. 
This helped us make sure we covered all important topics.
Unstructured Interviews: We asked open-ended questions, which let users share 
their thoughts in their own words. This helped us discover ideas that we might not 
have found with the structured questions.
##### • Key Findings:
Users felt frustrated by the huge number of movies available. They really wanted 
personalized recommendations that fit their own viewing history and likes. They also 
wanted features that let them browse movies by genre and rate films to help improve 
suggestions.
#### 2. Questionnaires:
##### • Purpose:
To gather quantitative data on user preferences and experiences, a questionnaire was 
distributed to a larger audience.
##### • Process:
The questionnaire was made by using google forms and was shared to many people to 
know about their recommendations and experiences.
##### • Key Findings:
The questionnaire gathered insights from 20 participants about their movie-watching 
habits and preferences. Most respondents watch 0-1 movie per week, with a 
preference for late-night viewing. Key findings highlighted a strong interest in Action 
and Animation genres, along with a desire for improved recommendation services 
based on ratings and peer suggestions.
#### 3. User Observation:
##### • Purpose:
Observing users while they searched for movies helped identify pain points and areas 
for improvement in the movie discovery process.
##### • Process:
Selected users were invited to use existing streaming platforms to find movies. 
Observers noted their behaviors, comments, and frustrations during the search 
process.
##### • Key Findings:
Users often spent a considerable amount of time scrolling through lists without 
finding suitable options.
Many users relied heavily on external reviews or friends’ recommendations, 
indicating a gap that the new system could fill.
### ➢ Analysis of Requirements:
After gathering data through these techniques, the information was analyzed to 
identify common themes and critical requirements. The analysis focused on:
#### 1. User Needs:
#### • Personalized recommendations.
#### • Easy navigation and browsing options.
#### • Social sharing capabilities.
#### 2. System Features:
#### • User profiles to track viewing history and ratings.
#### • A robust recommendation engine leveraging collaborative filtering.
#### • Real-time updates of recommendations based on user activity.
#### 3. Data Management:
#### • A comprehensive database structure to store user profiles, movie details, ratings, and watch history.
#### • Implementing auto-correction features for user input to enhance data accuracy

## 4. Database Design

### ⚫ Entities and Tables
#### ◆ Users Table
Purpose: Stores user profile information.
#### ◆ Movies Table
Purpose: Stores information about movies.
#### ◆ Ratings Table
Purpose: Collects ratings given by users for movies.
#### ◆ Genres Table
Purpose: Stores information about movie genres.
#### ◆ Watch History Table
Purpose: Tracks the movies that users have watched.
#### ◆ Recommendations Table
Purpose: Stores the movie recommendations generated for users.
#### ◆ Spelling Corrections Table
Purpose: Stores common spelling corrections for user inputs.
### ➢ Relationships
#### ◆ Users and Ratings:
Each user can provide multiple ratings for different movies, creating a one-to-many 
relationship between users and ratings.
#### ◆ Movies and Ratings: 
Each movie can receive ratings from multiple users, establishing a one-to-many 
relationship between movies and ratings
#### ◆ Movies and Genres:
Each movie belongs to one genre but can receive multiple ratings from different users.
#### ◆ Users and Watch History:
Each user can have multiple entries in their watch history, linking users to the movies 
they've watched.
### -> System Boundary Diagram
<img width="447" alt="image" src="https://github.com/user-attachments/assets/d931c57a-4000-4273-a2b4-b86a9c635386">

### -> User Views and Data Cross-Reference Table
<img width="366" alt="User View Table" src="https://github.com/user-attachments/assets/b99a26f9-8d58-44e1-a157-2ef4da518ef6">

### -> Cross Reference Table
<img width="419" alt="image" src="https://github.com/user-attachments/assets/97a6162a-9451-4c18-ae0e-5e05b8673014">

Mark sign indicates that the user view utilizes or interacts with that type of data.
#### ⚫ User Profile:
Users can manage their information, see their watch history, preferences, and ratings.
#### ⚫ Movie Recommendations:
This view primarily relies on user ratings to generate personalized recommendations.
#### ⚫ Movie Browsing:
Users can filter and browse movies by genre or search by title, and they can view 
ratings for these movies.
#### ⚫ Social Features:
This view allows users to share recommended movies with friends, enhancing social 
interaction.
#### ⚫ Admin Dashboard:
Administrators can access and manage user information, watch histories, and ratings.
#### ⚫ Search Functionality:
Users can search for movies by title or genre, enhancing their browsing experience.

### ➢ Auto Spelling Correction Implementation
#### ◆ Feature Design:
1. Utilize the Spelling Corrections table to store a dictionary of common 
misspellings and their corrections.
2. When users input text (such as movie titles or reviews), the system checks against 
this table for any misspellings.
3. The system can either automatically correct the misspellings in real-time or 
suggest corrections to users before they submit their input, enhancing data 
accuracy.
## 5. DBMS Selection 
 ### Two Types of Databases: RDBMS And NoSQL
#### RDBMS (Relational Databases,  MySQL ):
Works with organized data (like tables with movie details and user ratings).
Data is in a fixed structure, so it's easy to organize.
Best for smaller systems or if data structure doesn’t change often.
#### NoSQL (MongoDB):
Great for large, flexible, and changing data (like user reviews or movie suggestions).
Can handle huge amounts of data easily.
Works well if the system needs to grow quickly

## 6. Application Design

### a. Components:
##### Frontend (UI): Displays movie recommendations, ratings, and search results.
##### Backend : Handles user management, movie data, and recommendation logic.
##### Database: Stores user profiles, movie details, ratings, and recommendations.
### b. User Flow:
##### Login/Register: Users create an account or log in.
##### Profile Setup: Users provide preferences (favorite genres).
##### Rate Movies: Users rate movies they’ve watched.
##### Recommendations: The system suggests movies based on ratings and preferences.
##### Movie Details: Users can see details, watch trailers, or read reviews.
### c. Key Features:
##### Movie Recommendation Engine: Suggests movies based on user ratings.
##### Search & Filter: Search movies by genre, rating, etc.
##### Rating System: Users rate movies.
##### Movie Details: Shows information like cast, description, and reviews.
### d. Recommendation Algorithm:
 ##### Collaborative Filtering: Suggest movies liked by similar users.
 ##### Content-Based Filtering: Suggest movies based on movie features (e.g., genre).
### e. Tech Stack:
 Database: MySQL/MondoDB.
### f. Basic Flow:
User Interaction → Store ratings and preferences → Generate recommendations → Display recommendations.
## 7. Prototyping
### Designing the Pages (UI)
#### Home Page: Shows movies and a search bar.
#### Movie Details Page: Shows more info about a movie.
#### Profile Page: Lets users set preferences.
#### Recommendations Page: Shows movie suggestions.
### Seting Up the Backend
#### User Management: Allow users to register and log in.
#### Store Movie Data: Include basic movie info like title, genre, and description.
#### Recommendation System: Start simple – suggest movies based on what the user has rated highly.
### Creating the Database
#### Store:
User Information: Name, email, preferences.
#### Movies: 
Title, genre, rating.
#### Ratings: 
User ratings for movies.
#### Build Simple Recommendations
### Use basic logic:
Recommend movies based on similar genres or what other users liked.
### Connect Everything
Link the frontend (UI) with the backend  so that data like movies and recommendations can be shown to users.
### Test the Prototype:
#### User logs in and rates a few movies.
#### The system shows movie suggestions based on their ratings.
#### User can search for other movies.
