# Instagram-application
InstagramProject is a RESTful API for a simplified version of Instagram.

## Technologies Used
- Java
- Spring Boot
- Hibernate
- Jakarta Persistence API (JPA)
- MySQL
- Maven

## API Documentation
The InstagramProject API provides the following endpoints:
### Admin Controller
- Toggle Blue Tick: PUT /admin/user/{id}/{blueTick}
- Toggles the blue tick status of a user.
### Comment Controller
- Add Comment: POST /comment
- Adds a comment to a post.
### Post Controller
- Add Post: POST /post?email={email}&token={token}
- Adds a new post.
- Get All Posts: GET /post?email={email}&token={token}
- Retrieves all posts.
- Get Likes for Post: GET /post/{postId}/likeCount
- Retrieves the number of likes for a post.

### User Controller
- Sign Up: POST /user/signup
- Creates a new user account.
- Sign In: POST /user/signin
- Authenticates user and generates a token.
- Sign Out: DELETE /user/signout?email={email}&token={token}
- Logs out a user and invalidates the token.
- Update User: PUT /user?email={email}&token={token}
- Updates user information.
- Follow User: POST /user/follow/{myId}/{otherId}
- Follows another user.
- Like Post: POST /user/like
- Likes a post.

## Data Models
The InstagramProject API uses the following data models:
- Admin
- AuthenticationToken
- InstagramComment
- InstagramFollower
- InstagramFollowing
- Post
- PostLike
- User

## Summary
InstagramProject is a Java-based RESTful API that provides functionality similar to Instagram. It allows users to sign up, sign in, add posts, like posts, follow other users, and interact with comments. The API is built using Spring Boot, Hibernate, and MySQL, providing a robust and scalable solution for managing user accounts, posts, and social interactions.
