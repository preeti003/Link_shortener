# URL Shortener

![URL Shortener Logo](logo.png)

## Overview

URL Shortener is a web application that allows users to create shortened URLs for long web addresses. This project is built using Node.js, Express.js, MongoDB, and the "shortid" library.

## Features

- Generate Short URLs: Users can enter a long URL, and the application will generate a unique, shortened URL that redirects to the original long URL.
- Analytics: Users can view analytics for each shortened URL, including the total number of clicks and a visit history with timestamps.

## Installation

1. Clone the repository to your local machine using `git clone`.

2. Install dependencies by running `npm install`.

3. Set up a MongoDB database either locally or using a cloud service.

4. Configure the MongoDB connection URL in the application. Open `config.js` and replace `MONGODB_URI` with your MongoDB connection URL.

## Usage

1. Start the application by running `npm start`.

2. Access the application through your web browser at `http://localhost:3000`.

3. To create a new shortened URL, enter a long URL in the input field on the homepage and click the "Generate" button. The application will display the shortened URL.

4. To view analytics for a specific shortened URL, append `/analytics/:shortId` to the base URL, where `:shortId` is the short ID generated for the URL. For example: `http://localhost:3000/analytics/abc123`.

## API Endpoints

- `POST /`: Endpoint for generating a new short URL. Requires a request body with a `url` field containing the original long URL.

- `GET /analytics/:shortId`: Endpoint for retrieving analytics for a specific short URL. Replace `:shortId` with the short ID of the URL.

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose (ODM for MongoDB)
- shortid (Library for generating short IDs)

Feel free to customize the README with any additional information about your project. Provide details about how to contribute, any known issues, or additional usage instructions if needed. A comprehensive README helps users and contributors understand your project and how to use it effectively.
