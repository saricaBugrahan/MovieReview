### Project Overview

This project is a basic Java-based application for managing movies and their reviews. It utilizes Spring Boot framework and MongoDB for data storage. Below is a brief description of each file in the project:

---

#### Files:

1. **Movie.java**
   - This file defines the `Movie` class which represents a movie entity.
   - It includes various attributes like id, IMDb id, title, release date, trailer link, poster, genres, backdrops, and review IDs.
   - Annotations from Lombok and Spring Data MongoDB are used for generating boilerplate code and defining MongoDB collection mappings.

2. **MovieController.java**
   - This file implements the REST API endpoints related to movies.
   - It includes methods for retrieving all movies and a single movie by IMDb ID.

3. **MovieRepository.java**
   - This file defines the repository interface for performing CRUD operations on movies.
   - It extends the `MongoRepository` interface provided by Spring Data MongoDB.

4. **MoviesApplication.java**
   - This is the main class of the application that bootstraps the Spring Boot application.

5. **MovieService.java**
   - This file contains the service layer logic for movie-related operations.
   - It interacts with the `MovieRepository` to fetch movie data.

6. **Review.java**
   - This file defines the `Review` class representing a review entity.
   - It includes attributes such as id and body.
   - Annotations for Lombok and Spring Data MongoDB are used for code generation and MongoDB mappings.

7. **ReviewController.java**
   - This file implements the REST API endpoints for managing reviews.
   - It includes a method for creating a new review.

8. **ReviewRepository.java**
   - This file defines the repository interface for CRUD operations on reviews.
   - It extends the `MongoRepository` interface provided by Spring Data MongoDB.

9. **ReviewService.java**
   - This file contains the service layer logic for review-related operations.
   - It interacts with the `ReviewRepository` for review data manipulation.
   - It also updates the associated movie with the new review ID when a review is created.

---
