# Bivouac

Stack: Node JS, Express JS, MongoDB, Mongoose, EJS

# Features
. Responsive web design (RWD)</br>
. User authentication (Login/Register/Logout) and authorization (Post/Like/Edit)</br>
. Flash messages responding to users' interaction</br>
. Refactored with ES6 and ES7 syntax (eg: async/await)</br>
. RESTful API</br>

-------------------------------------------------------------------------
Normal Routes
-------------------------------------------------------------------------
[Method]  [Route]
GET       /                       Landing page
GET       /login                  Request the user login page
GET       /register               Request the user edit page

-------------------------------------------------------------------------
Users Route
-------------------------------------------------------------------------
[Method]  [Route]
GET       /users                  Fetch all users
POST      /users                  Create new user in database
GET       /users/new              Request the user register page
GET       /users/:id              Show the user information
PATCH     /users/:id              Update user information
DELETE    /users/:id              Delete user information
GET       /users/:id/edit         Request the user edit page

-------------------------------------------------------------------------
Sessions Route
-------------------------------------------------------------------------
[Method]  [Route]
POST      /sessions               Create a session (user login)
GET       /sessions/login         Request the user login page
DELETE    /sessions               Delete a session (user logout)

-------------------------------------------------------------------------
Campgrounds Route
-------------------------------------------------------------------------
[Method]  [Route]
GET       /campgrounds            Fetch all campgrounds
POST      /campgrounds            Create a new campground to database
GET       /campgrounds/new        Request the campground adding page
GET       /campgrounds/:id        Show the campground information
PUT       /campgrounds/:id        Update campground information (all)
PATCH     /campgrounds/:id        Update campground information (part)
DELETE    /campgrounds/:id        Delete a campground
GET       /campgrounds/:id/edit   Request the campground editing page
POST      /campgrounds/:id/likes  Like the campground

-------------------------------------------------------------------------
Comments Route
-------------------------------------------------------------------------
[Method]  [Route]
POST      /campgrounds/:id/comments       Create a new comment
PATCH     /campgrounds/:id/comments/:cid  Update comment
DELETE    /campgrounds/:id/comments/:cid  Delete comment

# Npm Packages
##### Cloudinary
##### Connect-flash
##### dotenv
##### ejs
##### ejs-mate
##### express
##### express-mongo-sanitize
##### express-session
##### helmet
##### joi
##### mongoose
##### multer
##### nodemon
##### passport
##### sanitize-html

# Gallery

## HomePage
![Screenshot 2023-03-14 131602](https://user-images.githubusercontent.com/97042529/224932149-0f4534ce-b9ee-4e75-bbf3-65e786a6f503.png)

## MainPage
![mp](https://user-images.githubusercontent.com/97042529/224933023-42cb56ed-e4db-42a9-b85b-16bbd3179e18.png)

## Campgrounds Page
![cp](https://user-images.githubusercontent.com/97042529/224933240-8eb5668d-11d8-4b24-a979-413dd8fb6204.png)

## Login Page
![Screenshot 2023-03-14 131725](https://user-images.githubusercontent.com/97042529/224932350-c14b62e6-7d2e-4242-a2fe-16fc327ff58e.png)

## Register Page
![rp](https://user-images.githubusercontent.com/97042529/224933360-77e8b912-960a-401a-9721-df090e581e29.png)

## New Campground Page
![ncp](https://user-images.githubusercontent.com/97042529/224933542-ab375303-7035-4198-81f0-ec9dd8430b0a.png)

## Edit Campground Page
![ecp](https://user-images.githubusercontent.com/97042529/224933608-c5810ce7-b381-4be5-9c1e-fe1ae5f3bd98.png)

## Deletion and Add Stars and Comments Page
![dr page](https://user-images.githubusercontent.com/97042529/224933716-aed8baf9-5a27-44cb-baed-0ddd9b8e019d.png)


