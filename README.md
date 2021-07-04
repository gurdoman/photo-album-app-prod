# Photo album app

This project is a Coding challenge for League

## User stories

1. As a user, I would like to see a list of my own albums along with their titles.
2. As someone interested in a particular album, I would like to see thumbnails of the photos in an album along with their titles.
3. As a user, I want to search for photo titles for a specific string. I would like the results returned to have the entire word italicized that matches the search parameter. Consider only single word search use cases and assume no special characters beyond just alphabetical characters. For example:
   1. If I were to search for "accu", the results would show the entire word "*accusamus*" as italicized.
   2. If I were to search for "fun" and there's a title with "refunds are not a fun time", the title would be displayed as "*refunds* are not a *fun* time". Both the word "refunds" and the word "fun" would be italicized. 
   3. If I were to search for "fun", a string with the following substring would **not** be italicized "...fu n..."

## Changes suggested to user stories

1. Changed album page from a list view to a grid view with a cover image as a link to the album
2. Search bar works for both albums and photos.
3. Search bar only works on the current page and gets cleared when you navigate out of the page

## Framework

Framework used was React, although I don't have that much experience with React I thought it would be a good idea for me to refresh my knowledge and for the coding challenge to be made in React since League builds their stuff on React.

## Architecture

Each component is inside of the components folder, each component works as a standalone, to be able to use them you need to import the models included in the components.

For calls to the server I created a service layer, this layer could have as many different services as we might need, for the moment I added the urls as private attributes but it could be reworked to send the url as a parameter and to create generic calls to the server. 

Inside each file you will see JSDoc type documentation and some suggestions for changes.

## How to run

This project is a simple React project, to run you need to:

### `npm install`

Installs all dependencies

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### `npm test`

Launches the test runner in the interactive watch mode.

## Author

Adrian Rossino
