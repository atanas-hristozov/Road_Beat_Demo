RidePal Web Application - Frontend Documentation
RidePal is a web application that creates personalized playlists tailored to users' musical preferences and trip durations. It integrates external APIs such as Microsoft Bing Maps and Deezer to determine travel times and fetch music data, allowing users to generate and manage playlists within the platform.

Frontend Overview
The frontend of RidePal is designed using modern web technologies and follows good practices in UI/UX to ensure a seamless user experience. Below is a detailed breakdown of the frontend structure and functionalities.

Table of Contents
Technologies Used
Core Functionalities
Public Section
Private Section
Administration Section
External Services
Installation
Developed By
Technologies Used
The frontend is built using the following technologies:

HTML5, CSS3, and LESS: For responsive design and styling
JavaScript: For dynamic content updates and interactive elements
Thymeleaf: As the templating engine integrated with Spring MVC
AJAX: For asynchronous requests and real-time playlist generation
REST API Integration: To communicate with backend services for playlist generation, authentication, and other actions
Core Functionalities
1. Playlist Generation
Users can generate a playlist by inputting:

Start and Destination Locations: Select between traveling by car or foot
Music Genres: Choose genres to customize the playlist
RidePal calculates the travel time using the Bing Maps API and fetches tracks from Deezer, creating a playlist whose duration matches the trip. The playlist can then be saved under the user's profile for future listening.

2. Playlist Browsing
Browse playlists created by other users
Filter by genre, duration, and average rank
Playlists are displayed in descending order based on average rating by default
Public Section
This section is available to all users, including non-authenticated visitors.

Homepage: Users can explore playlists and view basic site information.
Register/Login Pages: Visitors can register for a new account or log in to access additional features.
Browse Playlists: Unauthenticated users can browse and filter playlists by genre and duration.
Private Section
Once logged in, users have access to the following features:

Generate Playlists: Create a new playlist based on trip details.
Edit/Delete Playlists: Modify or remove playlists they own.
User Profile Management: Users can edit their profile details, including changing their profile picture.
Administration Section
System administrators have enhanced access and management capabilities:

Manage Users: View, edit, or delete user profiles and their associated playlists.
Manage Playlists: Admins can update or delete any playlist in the system.
User Privileges: Admins can control which users can manage playlists or perform specific actions.
External Services
The frontend interacts with the following external services:

Deezer API: Used to fetch music data such as tracks, albums, and genres to build playlists.
Microsoft Bing Maps API: Used to calculate the distance and travel duration between user-specified locations.
Installation
To install the frontend part of the RidePal application, follow these steps:

Clone the repository:
bash
Copy code
git clone https://github.com/atanas-hristozov/RidePal/tree/main/RidePal
Ensure the backend is set up and running (refer to the backend documentation for details).
Access the application on http://localhost:8080 in your web browser.
Developed By
Atanas Hristozov
Rosen Yanev
For more information or to contribute, visit the RidePal GitHub repository.
