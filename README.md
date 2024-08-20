# Puppeteer Automation Tool

## Overview

This project uses [Puppeteer](https://github.com/puppeteer/puppeteer), a Node.js library, to automate interactions with web applications. The tool performs tasks such as logging into a web application, navigating through pages, updating user profiles, and submitting job applications.

## Features

- Automated login to web applications
- Dynamic navigation through pages
- Form submissions with data from external sources
- Profile management (education, training, work samples)
- Application submission with pre-defined responses

## Prerequisites

- [Node.js](https://nodejs.org/) (v12 or later)
- [npm](https://www.npmjs.com/) (v6 or later)

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/puppeteer-automation-tool.git
   cd puppeteer-automation-tool

   
   npm install
## Configuration
Create a secret.js file:

Create a secret.js file in the root directory and include your credentials:
```bash
  module.exports = {
    id: 'your-email@example.com',
    pass: 'your-password'
  };
module.exports = [
    {
        "College": "Your College Name",
        "Degree": "Your Degree",
        "Stream": "Your Stream",
        "Percentage": "Your Percentage",
        "Training": "Your Training Name",
        "Organization": "Organization Name",
        "description": "Description of the training",
        "link": "Your Portfolio Link",
        "hiringReason": "Why should we hire you?",
        "availability": "Your availability",
        "rating": "Your self-rating"
    }
];
```
## Usage
To run the automation script, use the following command:
```


node index.js
```
The script will launch a new browser window (non-headless mode) and start automating the tasks. 
It will:<br>
1.Log in to the Unstop website.<br>
2.Navigate to the profile section and update the graduation details.<br>
3.Add training experiences.<br>
4.Upload work samples.<br>
5.Apply to internships listed on the Grand Summer Internship Fair page.<br>
<br><br>
## Script Structure<br>
1.main(): The main function that orchestrates the entire automation process.<br>
2.graduation(data): Fills in graduation details like college, degree, and stream.<br>
3.training(data): Adds details about training experiences.<br>
4.workSample(data): Uploads a work sample or portfolio link.<br>
5.application(data): Navigates to the internship fair page and applies to available internships.<br>
6.apply(url, data): Fills in the application form for each internship.<br>






