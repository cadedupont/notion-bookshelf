# Notion Bookshelf

JavaScript program to query Google Books API for a book title passed as a command line argument and get all book properties from the API response. The program then creates a new page in a Notion database and adds the book properties to that page.

### Setting up API keys
Before attempting to run the program, ensure that you have a Notion database present in your workspace.

You will need to install Node.js on your machine and create a `.env` file in the root directory of the project containing the following:

```
NOTION_TOKEN=your_key_here

NOTION_DATABASE_ID=your_key_here

GOOGLE_BOOKS_API_KEY=your_key_here
```

Replace every instance of `your_key_here` with the corresponding [Notion](https://developers.notion.com/) and [Google Books](https://developers.google.com/books/docs/overview) API keys. The `NOTION_DATABASE_ID` is a string of letters and numbers identifying the database in the URL. A short guide to finding this string can be found [here](https://stackoverflow.com/a/69860478).

### To run
The program is currently configured to run using Node.js. Run the following command at the project's root directory to install dependencies from the `package.json` file:<br>

`npm install`

Then, to run the JavaScript file using the Node.js interpreter, run the following command:<br>

`node main.js '<insert book title>'`<br>

Replace `'<insert book title>'` with the title of the book you are looking to search for. Make sure to wrap the title in either single quotes or double quotes so the program can parse the command line arguments as intended.

---
<p align='center'>
  <img width="1102" alt="gallery" src="https://github.com/cadedupont/notion-bookshelf/assets/98860495/7f2674e0-c43a-4d73-991b-fa126c5b5e4d">
  <img width="957" alt="page" src="https://github.com/cadedupont/notion-bookshelf/assets/98860495/ee6ca720-91a8-45d0-ae7d-1e6b97a5aa02">
</p>
