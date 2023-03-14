
# Bivouac

A website for reviewing campgrounds by using the data of users such as their geographic location to gather information about the campgrounds they have visited. This data is stored as per each user. The user can post the review for campgrounds which can be public can can be viewed by registered users. One of the major aspect of the website is to keep the data of the user private. This website is packed with security features to meet the expectations of privacy and security.
## Features

- Responsive web design (RWD)
- User authentication (Login/Register/Logout) and authorization (Post/Like/Edit)
- Flash messages responding to users' interaction
- Refactored with ES6 and ES7 syntax (eg: async/await)
- RESTful API



## API Reference

#### Normal Routes

```http
  GET /                  Landing Page
```
#### Authentication Routes

```http
  GET /login             Login Page
  GET /register          Register Page
```

#### Users Routes

```http
  [Method]  [Route]
  GET       /users             Fetch all users
  POST      /users             Create new user in database
  GET       /users/new         Request the user register page
  GET       /users/:id         Show the user information
  PATCH     /users/:id         Update user information
  DELETE    /users/:id         Delete user information
  GET       /users/:id/edit    Request the user edit pag
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `email` | `string` | **Required**. Email is Required|
| `password` | `string` | **Required**. Password is Required|
| `user_id` | `string` | **Required**. user_id is Required|


#### Campgrounds Route

```http
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
```

#### Comments Route

```http
[Method]  [Route]
POST      /campgrounds/:id/comments       Create a new comment
PATCH     /campgrounds/:id/comments/:cid  Update comment
DELETE    /campgrounds/:id/comments/:cid  Delete comment
```

## Tech Stack

**Client:** Bootstrap, EJS

**Server:** Node, Express, MongoDB


## Screenshots

#### Home Page
![Screenshot 2023-03-14 131602](https://user-images.githubusercontent.com/97042529/224932149-0f4534ce-b9ee-4e75-bbf3-65e786a6f503.png)

#### Main Page
![mp](https://user-images.githubusercontent.com/97042529/224933023-42cb56ed-e4db-42a9-b85b-16bbd3179e18.png)

#### Login Page
![Screenshot 2023-03-14 131725](https://user-images.githubusercontent.com/97042529/224932350-c14b62e6-7d2e-4242-a2fe-16fc327ff58e.png)

#### Register Page
![rp](https://user-images.githubusercontent.com/97042529/224933360-77e8b912-960a-401a-9721-df090e581e29.png)

#### New Campground Page
![ncp](https://user-images.githubusercontent.com/97042529/224933542-ab375303-7035-4198-81f0-ec9dd8430b0a.png)

#### Edit Campground Page
![ecp](https://user-images.githubusercontent.com/97042529/224933608-c5810ce7-b381-4be5-9c1e-fe1ae5f3bd98.png)

#### Deletion and Add Stars and Comments Page
![dr page](https://user-images.githubusercontent.com/97042529/224933716-aed8baf9-5a27-44cb-baed-0ddd9b8e019d.png)




