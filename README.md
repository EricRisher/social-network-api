
  # Social Network API

   ## Table-of-Contents

  * [Description](#description)
  * [Installation](#installation)
  * [Usage](#usage)
  * [License](#license)
  * [Contributing](#contributing)
  * [Tests](#tests)
  * [Questions](#questions)
 

  ## Description
  My motivation for creating this Social Network API stemmed from a keen interest in exploring the capabilities of NoSQL databases, particularly MongoDB, in handling the dynamic and unstructured data typical of social media platforms. This project offered a hands-on opportunity to apply Express.js and Mongoose in developing an API that mirrors the functionality of real-world social networks, highlighting the power and flexibility of MongoDB in managing large volumes of data efficiently.

  I built this project to explore MongoDB and gain experience with backend development for social networks, using Express.js and Mongoose. It was a practical way to understand how to manage unstructured data and implement key social networking features.

  This project solves the problem of efficiently managing and querying large amounts of unstructured data in a social networking context. It provides a scalable API that supports user interactions, such as sharing thoughts, reacting to posts, and managing friend lists, showcasing how NoSQL databases like MongoDB can handle complex data relationships and rapid scalability demands inherent in social media platforms.
 

  ## Installation
  To install this Social Network API project, follow these steps:

1. Clone the repository:  
   `git clone git@github.com:EricRisher/social-network-api.git`  

2. Navigate to the project directory:  

   `cd main`  

3. Install dependencies:  
  `npm install`  

4. Set up MongoDB:

   Ensure MongoDB is installed and running on your local machine. If not, download and install it from the official MongoDB website.   

5. Start the server:

   Once the dependencies are installed and MongoDB is running, start the project server with:

   `npm run start`  
This will launch the Express.js server, connecting it to your MongoDB database using Mongoose.  

6. Access the API:

   With the server running, you can now use API testing tools like Insomnia or Postman to interact with the API endpoints for users, thoughts, friends, and reactions.

  ## Usage
  To use the Social Network API with Postman, follow these instructions. This guide assumes you have Postman installed and the Social Network API server running locally on your machine.  


  Setting Up Postman
1. Launch Postman: Open the Postman application.  

2. Create a New Collection: Click on the "New" button, then select "Collection". Name your collection (e.g., "Social Network API") and save it.

Making Requests  

Create a New User:  

Method: POST  
URL: http://localhost:3000/api/users  
Body: Select raw and JSON format, then input the user data in JSON format.  
```
{
  "username": "newuser",
  "email": "newuser@example.com"
}
```
Send: Click the "Send" button to make the request.   

Get All Users  

Method: GET  
URL: http://localhost:3000/api/users  
Send: Click the "Send" button to retrieve all users.  

Add a Friend  
Method: POST  
URL: Replace userId with the user's ID to whom you want to add a friend and friendId with the friend's ID. http://localhost:3000/api/users/:userId/friends/:friendId  
Send: Click the "Send" button to add the friend.  

Create a Thought  
Method: POST  
URL: http://localhost:3000/api/thoughts  
Body: Select raw and JSON, then input the thought data.  
```
{
  "thoughtText": "Here's a cool thought...",
  "username": "newuser",
  "userId": "<user-id>"
}
```
Send: Click the "Send" button.   

Add a Reaction to a Thought  
Method: POST  
URL: Replace thoughtId with the ID of the thought you want to react to. http://localhost:3000/api/thoughts/:thoughtId/reactions  
Body: Select raw and JSON, then input the reaction data.  
```
{
  "reactionBody": "Wow, that's interesting!",
  "username": "anotheruser"
}
```
Send: Click the "Send" button.  


  ## Contributing
  None

  ## Tests
  None

  ## Questions
  If you have any questions, please contact me at 
  rishereric13@gmail.com
  or visit my GitHub page at
  [GitHub](https://github.com/ericrisher)

