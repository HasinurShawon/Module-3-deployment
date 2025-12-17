

## Prerequisites

- Node Version 22


### 1. For Run This Applications
```bash
# install packages
npm install 

# Testing The Applications
npm check

# For Run the application
npm start
```


### Deployment Process
1. **Cleanup**: Removes existing process if running
   ```bash
   pm2 delete node-app || true
   ```

2. **Start Application**: Launches with absolute path
   ```bash
   pm2 start "./src/server.js" --name node-app
   ```

3. **Save Process List**: Persists PM2 configuration
   ```bash
   pm2 save
   ```

### About The Applications
1. **Route**: This Application has 2 route
   ```bash
   / # this will show a hello world page
   ```
      ```bash
   /api # this will response a json
   ```

2. **Default Port**: By Default this application will run on port 3000

Assignment on module 3
Assignment: Deploy a Website on AWS EC2
Project Repository:
https://github.com/roy35-909/Module-3-deployment.git

Objective
Deploy a Node.js web application on an AWS EC2 instance and document each step with screenshots.

Tasks
Step 1: Clone the Repository on Your Local Machine
●Clone the provided GitHub repository into your local system.


●Open the project folder.


●Take a screenshot showing the cloned repository.


Step 2: Run and Test the Application Locally
●Install the project dependencies.


●Run the application on your local machine.


●Test if the app works in your browser.


●Take screenshots showing the app running locally.


Step 3: Create an EC2 Instance (t3-medium)
●Log in to AWS and create a new EC2 instance.


●Choose instance type t3-medium.


●Configure security groups to allow necessary ports.


●Launch the instance.


●Take a screenshot of the instance running.


Step 4: Connect to the EC2 Instance
●Connect to the instance using SSH or PuTTY.


●Take a screenshot showing the successful connection.


Step 5: Clone the Repository on the EC2 Instance
●Install Git if needed.


●Clone the same GitHub repository onto your EC2 machine.


●Take a screenshot showing the cloned project on EC2.


Step 6: Install Node.js and Project Dependencies
●Install Node.js on the EC2 instance.


●Install the project’s npm packages.


●Take a screenshot showing Node.js installed and dependencies completed.


Step 7: Run the Application in the Background
●Use any background process tool (example: pm2, screen, nohup).


●Start the application so it continues running even after closing the terminal.


●Take a screenshot of the background process running.


Step 8: Run the Application on the EC2 Instance
●Ensure the application is running and accessible.


●Use the EC2 public IP to test the application in your browser.


●Take a screenshot of the app running from EC2.


Step 9 (Optional): Configure NGINX as a Reverse Proxy
●Install and configure NGINX to forward traffic to your Node.js application.


●Access the app using EC2’s public IP (without a port).


●Take a screenshot if you complete this step.


Submission Guidelines
●Create a Google Docs file.

●Add screenshots for every step listed above.

●Ensure each screenshot includes a short description of what you did.

●Submit the link to the Google Doc.


