# RidePal Web Application - Frontend Documentation

RidePal is a web application designed to create personalized playlists based on users' music preferences and trip durations. The app integrates external APIs such as Microsoft Bing Maps for calculating travel times and Deezer for fetching music data. It builds custom playlists that match users' travel duration within the platform.

![Home Page](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/Home_Page.JPG)

## Table of Contents
- [Technologies and Principles](#technologies-and-principles)
- [Main Functionalities](#main-functionalities)
- [Public Part](#public-part)
- [Private Part](#private-part)
- [Administration Part](#administration-part)
- [REST API](#rest-api)
- [External Services](#external-services)
- [Database](#database)
- [Installation](#installation)
- [Developed By](#developed-by)

## Technologies and Principles
- **Languages and Frameworks**: Java, Spring Boot, Spring MVC, Thymeleaf, HTML, CSS, LESS, JavaScript
- **Testing**: JUnit, Mockito
- **Database**: MariaDB
- **Additional Technologies**: Hibernate for ORM
- **Good Practices**: A well-defined layered architecture and over 80% test coverage in the service layer ensure maintainability and high-quality code.

## Main Functionalities

### 1. Playlist Generation
- Users input their starting and destination addresses, choose to travel by car or on foot, and select their preferred music genres.
- RidePal calculates the trip duration and generates a playlist from the chosen genres that matches the travel time.
- Playlists can be saved under the user's profile for later listening.

![Playlist Generation](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/Playlist.JPG)

### 2. Playlist Browsing
- Users can browse playlists created by other users.
- Playlists can be filtered by duration and genre.
- By default, playlists are sorted in descending order based on their average rank.

![All Playlists](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/All_Playlists.JPG)

## Public Part
This section is visible to all users, including those not authenticated.
- **Register/Login Pages**: Users can create a new account or log in.
- **Browse Playlists**: Visitors can browse playlists, filter them by genre and duration, and explore public playlists without logging in.

![Register Page](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/Register.JPG)

## Private Part
Users with an account can:
- **Generate Playlists**: Create new playlists based on travel data.
- **Edit/Delete Playlists**: Modify the title, cover image, or delete playlists they own.
- **Profile Management**: Users can update their profiles, including profile pictures.

![Generate Playlist](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/Generate.JPG)

## Administration Part
System administrators have additional permissions beyond regular users, such as:
- **Manage Users**: View all users and update or delete user profiles and their associated playlists.
- **Manage Playlists**: Admins can update or delete any playlist in the system.

![My Profile](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/My_Profile.JPG)

## REST API
The RidePal application exposes a REST API that can be accessed at:
- **Base URL**: `http://localhost:8080` (once configured)

## External Services
RidePal relies on the following external APIs for playlist generation and travel time calculations:
- **Deezer API**: Used to fetch tracks, genres, albums, and artists. [Deezer API Documentation](https://developers.deezer.com/api)
- **Microsoft Bing Maps API**: Used to calculate the distance and travel duration between two waypoints based on coordinates. [Bing Maps API Documentation](https://www.microsoft.com/en-us/maps/bing-maps/distance-matrix)

## Database
- **MariaDB** is the relational database used for storing user information, playlists, and other data relevant to the system.

## Installation

### Prerequisites
- **Java Development Kit (JDK)**
- **MariaDB** installed and configured on your machine.

### Steps:
1. Clone the project from the following GitHub repository:
   ```
   git clone https://github.com/atanas-hristozov/RidePal/tree/main/RidePal
   ```
2. Configure the database connection settings in the `application.properties` file.
3. Run the two SQL scripts in the `DB` folder inside `src` to create the database and populate it with initial data.
4. You do not need an API key to run the project locally.
5. Once everything is set up, access the web application at:
   ```
   http://localhost:8080
   ```

## Developed By
- **Atanas Hristozov**
- **Rosen Yanev**

![About](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/About.JPG)
