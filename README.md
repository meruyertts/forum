
## ABOUT:

This project consists in creating a web forum that allows :

    communication between users.
    associating categories to posts.
    liking and disliking posts and comments.
    filtering posts.

_SQLite_

In order to store the data in this forum (like users, posts, comments, etc.) SQLite database library is used.

SQLite is a popular choice as an embedded database software for local/client storage in application software such as web browsers. It enables you to create a database as well as controlling it by using queries.


_Authentication_

In this segment the client must be able to register as a new user on the forum, by inputting their credentials. A login session is created to access the forum and be able to add posts and comments.

Cookies are used to allow each user to have only one opened session. Each of this sessions must contain an expiration date.

Instructions for user registration:
    Must ask for email
        When the email is already taken return an error response.
    Must ask for username
    Must ask for password
        The password must be encrypted when stored (this is a Bonus task)

The forum must be able to check if the email provided is present in the database and if all credentials are correct. It will check if the password is the same with the one provided and, if the password is not the same, it will return an error response.

_Communication_

In order for users to communicate between each other, they will have to be able to create posts and comments.

    Only registered users will be able to create posts and comments.
    When registered users are creating a post they can associate one or more categories to it.
        The implementation and choice of the categories is up to you.
    The posts and comments should be visible to all users (registered or not).
    Non-registered users will only be able to see posts and comments.

_Likes and Dislikes_

Only registered users will be able to like or dislike posts and comments.

The number of likes and dislikes should be visible by all users (registered or not).

_Filter_

A filter mechanism is implemented, that will allow users to filter the displayed posts by :

    categories
    created posts
    liked posts

You can look at filtering by categories as subforums. A subforum is a section of an online forum dedicated to a specific topic.

Note that the last two are only available for registered users and must refer to the logged in user.

_Docker_

For the forum project a Docker is used.

### Usage

run locally
```
make run 
```
run in docker 
```
make docker 
```
