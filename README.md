# Note Taker

## Description

Note Taker is an application that allows users to write, save, and delete notes. This application uses an Express.js back end and saves and retrieves note data from a JSON file.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Routes](#api-routes)
- [Deployment](#deployment)
- [Acceptance Criteria](#acceptance-criteria)
- [License](#license)

## Installation

1. Clone the repository to your local machine:
   bash
   git clone https://github.com/your-username/note-taker.git
   cd note-taker
   

2. Install the necessary dependencies:
   bash
   npm install
   

## Usage

1. Start the server:
   bash
   node server.js
   

2. Open your browser and go to `http://localhost:3001` to use the application.

## API Routes

### HTML Routes

- `GET /notes` - Returns the `notes.html` file.
- `GET *` - Returns the `index.html` file.

### API Routes

- `GET /api/notes` - Reads the `db.json` file and returns all saved notes as JSON.
- `POST /api/notes` - Receives a new note to save on the request body, adds it to the `db.json` file, and returns the new note to the client.
- `DELETE /api/notes/:id` - Receives a query parameter containing the id of a note to delete. Deletes the note with the given `id` property from the `db.json` file.

## Deployment

This application can be deployed on [Render](https://render.com/).

1. Push your project to a GitHub repository.
2. Sign up for Render and create a new Web Service.
3. Connect your GitHub repository to Render.
4. Specify the build and start commands:
   - Build Command: `npm install`
   - Start Command: `node server.js`
5. Deploy the application.

## Acceptance Criteria


GIVEN a note-taking application
WHEN I open the Note Taker
THEN I am presented with a landing page with a link to a notes page
WHEN I click on the link to the notes page
THEN I am presented with a page with existing notes listed in the left-hand column, plus empty fields to enter a new note title and the note’s text in the right-hand column
WHEN I enter a new note title and the note’s text
THEN a "Save Note" button and a "Clear Form" button appear in the navigation at the top of the page
WHEN I click on the Save button
THEN the new note I have entered is saved and appears in the left-hand column with the other existing notes and the buttons in the navigation disappear
WHEN I click on an existing note in the list in the left-hand column
THEN that note appears in the right-hand column and a "New Note" button appears in the navigation
WHEN I click on the "New Note" button in the navigation at the top of the page
THEN I am presented with empty fields to enter a new note title and the note’s text in the right-hand column and the button disappears


## License

This project is licensed under the MIT License.
