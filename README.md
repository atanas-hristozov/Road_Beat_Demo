# RidePal Web Application - Frontend Documentation (Demo Version)

This is a **demo** of the frontend for the RidePal web application, a platform designed to create personalized playlists based on users' music preferences and travel durations. The demo showcases the user interface and functionalities such as playlist generation, browsing, and user profile management. 

The demo does not include the backend services for playlist creation, user authentication, or data persistence but provides an overview of the key frontend features and interactions.

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
- Users can input starting and destination addresses, choose travel mode (car or foot), and select preferred genres.
- The demo shows how playlists would be generated based on travel duration, though the actual generation process is simulated in this frontend demo.

![Playlist Generation](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/Playlist.JPG)

### 2. Playlist Browsing
- Users can browse and filter playlists based on duration and genre.
- Sorting by average rank and filtering options are available, though backend integration is not included in this demo.

![All Playlists](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/All_Playlists.JPG)

## Public Part
The public part of the demo includes:
- **Register/Login Pages**: Users can view the registration and login interfaces.
- **Browse Playlists**: Visitors can explore playlists and filter by genre and duration, though interaction with a real database is not enabled.

![Register Page](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/Register.JPG)

## Private Part
In the demo, authenticated users can:
- **Generate Playlists**: Simulate playlist generation.
- **Edit/Delete Playlists**: View how they would manage their playlists in a fully functional version.
- **Profile Management**: Explore the user profile interface with options for editing and updating profile details.

![Generate Playlist](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/Generate.JPG)

## Administration Part
The demo allows administrators to:
- **Manage Users**: View user management interfaces, including profile editing and deletion options.
- **Manage Playlists**: Simulate playlist management features such as updating or deleting any playlist.

![My Profile](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/My_Profile.JPG)

## REST API
Although this demo frontend simulates interaction with the backend, in the full version, the RidePal application exposes a REST API that can be accessed at:
- **Base URL**: `http://localhost:8080` (available in the full application)

## External Services
In a fully functional version, the following external APIs would be used:
- **Deezer API**: Fetches music data (tracks, genres, albums). [Deezer API Documentation](https://developers.deezer.com/api)
- **Microsoft Bing Maps API**: Calculates distance and travel duration based on user inputs. [Bing Maps API Documentation](https://www.microsoft.com/en-us/maps/bing-maps/distance-matrix)

## Database
The full RidePal application uses **MariaDB** for storing user data and playlists. This demo does not include database integration.

## Installation

### Prerequisites
- **Java Development Kit (JDK)**
- **MariaDB** (for full backend integration)

### Steps:
1. Clone the project from the GitHub repository:
   ```
   git clone https://github.com/atanas-hristozov/RidePal/tree/main/RidePal
   ```
2. Follow instructions in the backend documentation for database and API configuration (not included in this demo).
3. Access the demo application at:
   ```
   http://localhost:8080
   ```

## Developed By
- **Atanas Hristozov**
- **Rosen Yanev**

![About](https://github.com/atanas-hristozov/RidePal/blob/main/RidePal/src/main/resources/static/img_documentation/About.JPG)
