Instagram Challenge
===================

## User stories

### Signing Up and Loggin In

* users can sign up with username, email, and password
* users can sign in with username or email, and password
* only valid email addresses can be entered for sign up
* visiters are always redirected to the sign up page if they aren't logged in

### Posting and Seeing Pictures

* users can post a picture
* users can post a description with the picture
* pictures show a username and timestamp
* users can delete their own pictures

### Interacting with Pictures
* users can like pictures
* users can comment on peoples pictures
* only the latest 2 comments are shown
* "View all N comments" will open a frame that shows the picture and comments

### Databases

#### Posts
| column | data type |
| -- | -- |
| id | int |
| user_id | int |
| description | string |
| time_posted | timestamp |
| time_edited | timestamp |
likes?

#### Comments
| column | data type |
| -- | -- |
| id | int |
| user_id | int |
| post_id | int |
| time_created | timestamp |
| comment | string |
comment likes?

### Users
whatever Devise wants, Devise can have. Devise is the star child here.


## Instructions

* Feel free to use Google, your notes, books, etc., but work on your own
* If you refer to the solution of another coach or student, please put a link to that in your README
* If you have a partial solution, **still check in a partial solution**
* You must submit a pull request to this repo with your code by 9am Monday morning

## Task

Build Instagram: Simple huh!

Your challenge is to build Instagram using Rails. You'll need **users** who can post **pictures**, write **comments** on pictures and **like** a picture. Style it like Instagram's website (or more awesome).

Bonus if you can add filters!

## How to start

1. Produce some stories, break them down into tasks, and estimate
2. Fork this repo, clone, etc
3. Initialize a new rails project

Remember to proceed in small steps! Getting confused? Make the steps even smaller.

## Code Quality

For linting, you can use the `.rubocop.yml` in this repository (or your own!).
You'll need these gems:

```ruby
gem "rubocop", "0.79.0", require: false
gem "rubocop-rails"
```

You can also lint Javascript, CSS, and ERB — feel free to research this. These
will help you to train yourself to produce cleaner code — and will often alert
you to mistakes or mishaps!
