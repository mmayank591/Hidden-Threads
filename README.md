# Hidden Threads
Hidden Threads is an innovative pseudonymous social platform designed to allow users to share their authentic experiences while keeping their true identities hidden. This enables users to freely express themselves without the fear of judgment. The app's primary goal is to foster a community where individuals can speak the truth, challenge societal norms, and explore different perspectives.


https://github.com/Rahul-chaurasiya/QuietNet/assets/77222540/0d35c3c2-0f3c-4ccb-b63f-24312bad357a


## Key Features

Registration Process:The registration process consists of several steps, such as signing up, creating a user profile, and confirming registration. During this process, users provide their pseudonymous username, email, and password, with the option to include additional profile information. These details are stored in the user table within the database.

Profile Management:Users have the ability to manage and update their profiles. This includes changing their pseudonymous username, updating their email, uploading a profile picture, and editing their bio. These changes are reflected in the user table of the database.

Main Feed:The main page features posts from all users. Users can browse through various topics and, upon clicking a post, can read the details and share their own thoughts. Posts are stored in the post table of the database, with each post linked to the user who created it using a foreign key pUserid.

Expressing Thoughts:Users are encouraged to share their thoughts on existing topics or introduce new topics if they don’t find one that resonates with them. When a user shares their thoughts, a new post is created and added to the post table in the database.

Like Feature:Users can like posts to show support or agreement with the content. Likes are stored in the like table of the database, with each like being connected to both the user who liked it and the post it is associated with.

Sign-In/Sign-Out System:Hidden Threads employs a secure sign-in and sign-out system for user authentication. This ensures that user accounts are protected and only authorized users can access the platform. Authentication is managed via session tokens or cookies.

Database Design and Relationships:The database is structured with several tables:

- The user table stores all user details and is linked to posts via the pUserid foreign key.
- The post table holds all posts made by users and references the user table through pUserid.
- The like table keeps track of which users liked which posts, with relationships to both the user and post tables.
- The comment table stores user comments on posts, creating links between users and posts.
