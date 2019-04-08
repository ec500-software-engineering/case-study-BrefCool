# Case study - Mastodon
## 1. Technology and Platform
### a. Coding language
### b. Building system
### c. Frameworks or libraries used
## 2. Testing
## 3. Software architecture
### a. How would you add/edit functionality to this project? How would one use this project from external projects?
### b. What part of the softwares are asynchronous?
### c. System diagram
Here's an overview of the Mastodon Instance:  
<img src="./images/Mastodon_Instance.PNG">  
Mastodon Instance can be deployed by anyone on any servers. All Mastodon Instances then can communicate with each other via ActivityPub protocol. Users can choose any one Mastodon Instance and register an account on it. Then users not only can view all the information published by users from this instance, but also can get information from other different instances.  
One Mastodon Instance consists several different modules: Nginx, PostgreSQL database, Redis, a web backend program written on Ruby and a streaming module developed on Node.js. The Nginx acts as a proxy which will handle all the HTTP requests from users. The PostgreSQL db is used for users' data storage. The Redis is used to cache data and to store queued tasks. The web application powers the REST API and all the web pages. The streaming module is used to GET or POST informations between different Mastodon instances.
### e. What architectural patterns are sued?

## 4. Analyze two defects in the project
## 5. Demo
I successfully install my own Mastodon Instance on a AWS EC2 VM. In order to let people visit my own Mastodon instance, I set up a domain for the AWS EC2 and then people can visit this instance by url: <https://www.brefcube.com>.
<img src="./images/website.PNG">