# JENKINS BUILD/UPGRADE LIVE DASHBOARD

## Project Overview
This project is a live dashboard that fetches job data from the Jenkins REST API. It provides real-time insights into build and upgrade progress, as well as automation progress. The dashboard is built using Node.js for the server-side operations and MongoDB for data storage.

## Features
- **User Authentication**: Login and signup pages.
- **Dashboard Views**: 
  - Build and upgrade progress.
  - Automation progress.
- **Data Fetching**: Utilizes Jenkins REST API to fetch job data.
- **Data Storage**: MongoDB for storing and retrieving data.
- **Progress Calculation**: Calculates progress percentage of builds and upgrades.

## Project Structure
project/
├── db/
│ └── schema.js
├── public/
│ ├── styles.css
│ ├── image.svg
│ └── script.js
├── views/
│ ├── login.ejs
│ ├── signup.ejs
│ ├── dashboard.ejs
│ └── page.ejs
├── jenkins.js
├── mongo.js
├── format.js
├── dashboardcalc.js
├── package.json
└── README.md


## Files and Directories
- **db/schema.js**: Defines the MongoDB schema for storing Jenkins job data.
- **public/**: Contains static files.
  - **styles.css**: Custom styles for the application.
  - **image.svg**: SVG image used in the application.
  - **script.js**: Client-side JavaScript for the application.
- **views/**: Contains EJS templates for rendering web pages.
  - **login.ejs**: Login page.
  - **signup.ejs**: Signup page.
  - **dashboard.ejs**: Dashboard page displaying build and upgrade progress.
  - **page.ejs**: Page displaying automation progress.
- **jenkins.js**: Server-side script that handles API requests to Jenkins and serves the application.
- **mongo.js**: Handles MongoDB connections and operations.
- **format.js**: Formats the date of builds.
- **dashboardcalc.js**: Calculates the progress percentage for builds and upgrades.
- **package.json**: Project dependencies and scripts.

## Getting Started
### Prerequisites
- Node.js
- MongoDB

### Installation
**1. Clone the repository:**
   ```bash
   git clone https://github.com/kavinraj13/motorolaintern.git
   cd project

2. Install dependencies:
   npm install

Set up MongoDB:
Ensure MongoDB is running and update the MongoDB connection string in mongo.js if necessary.

###Configure Jenkins API:
Update the Jenkins API URL and credentials in jenkins.js.
Running the Application
Start the server:
node jenkins.js
Open your browser and navigate to http://localhost:3000.


Usage
Login/Signup: Create an account or login with existing credentials.
Dashboard: View real-time progress of Jenkins jobs.
Build and upgrade progress is displayed on dashboard.ejs.
Automation progress is displayed on page.ejs.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
Jenkins
Node.js
MongoDB

Feel free to customize this README.md to better suit your project's specifics and add any additional information as needed.
Make sure to update any placeholder URLs and details with your actual information where needed.




