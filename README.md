# Console-based-Social-Network-Application-By-Using-OOP-Concepts

📌 Project Overview

This project implements a console-based social network system using Object-Oriented Programming (OOP) concepts in C++.
The application simulates a small-scale social media platform where:

Users can add friends

Like posts

Comment on posts

View timelines

View pages

Share posts

Search for users, pages, or posts

All entities (Users, Pages, Posts) are stored and managed using dynamic memory allocation, inheritance, and polymorphism.

🎯 Core Objectives

Practice OOP principles (Inheritance, Polymorphism, Encapsulation, Abstraction)

Implement dynamic memory allocation (DMA) without global variables

Handle file input and output for Users, Pages, and Posts

Simulate social network functionality through a clean console interface

Reproduce the required sample output using a SocialNetworkApp::Run() function

🏗️ System Components
🧩 1. SocialEntity (Base Class)

Common parent for:

User

Page

Contains shared attributes:

ID

Name

🧍 2. User Class

Each user has:

Unique ID & Name

Friend List (max 10)

Liked Pages (max 10)

Timeline posts

Ability to Like/Comment/Share posts

📄 3. Page Class

Each page has:

Unique ID & Title

A list of posts on its timeline

Can receive comments and likes from users

📝 4. Post Class

Each post contains:

Unique ID

Description / Text

PostedOn date

PostedBy pointer (User/Page)

Max 10 comments

Max 10 likes

Optional Activity:

Type	Meaning	Example Values
1	Feeling	happy, sad, excited
2	Thinking	life, future
3	Making	memories, art
4	Celebrating	birthday, success
💬 5. Comment Class

A comment contains:

CommentedBy (User/Page)

Text

Date

⚙️ Functional Requirements
✔ 1. Set Current User

Ask for user ID and set as active session user.

✔ 2. View Home

Display posts from:

Friends (last 24 hours)

Liked Pages (last 24 hours)

✔ 3. Like a Post

Like a post (max 10 likes allowed).

✔ 4. View List of People Who Liked a Post

Display all users/pages who liked a specific post.

✔ 5. Comment on a Post

Add a new comment to a post.

✔ 6. View a Post

Show full post + all comments.

✔ 7. Share a Post

Share an existing post on the current user’s timeline.

✔ 8. View User Timeline

Show:

User name

All timeline posts

✔ 9. View Friend List

Show all friends of a selected user.

✔ 10. View Page

Display all posts of a page.

✔ 11. Search

Search keyword in:

User names

Page titles

Post descriptions

🧠 OOP Requirements
✔ Inheritance

SocialEntity → { User, Page }

✔ Polymorphism

Specialized post types:

FeelingPost

ThinkingPost

MakingPost

CelebratingPost

Each overrides display behavior.

✔ Encapsulation

All data members private/protected.

✔ Abstraction

High-level public functions only (e.g., ViewHome(), LikePost()).

🔧 Memory Management

All arrays are dynamically allocated.

Use double pointers for arrays of objects.

If no friends or posts → pointers remain NULL.

Implement:

Copy Constructor

Assignment Operator

Destructor

📂 File Handling

The program reads data from files:

Users

Pages

Posts

Comments

Likes

The data is loaded at startup and saved on exit.
