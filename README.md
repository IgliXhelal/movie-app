# Movie App

A browser-based movie collection for the Web Technologies and Programming course. Browse the 20 movies from the original project, search by title or director, filter by genre, and view film details. Use **Manage** to add, edit, or delete movies and see the collection's rating and genre breakdown.

## Run the project

Open `index.html` or serve this directory with VS Code Live Server. The project uses plain HTML, CSS, and JavaScript. It requires no build, server, database, account, or API key. The original HTTPS poster links are used for images, with a placeholder if an image is unavailable.

Movies are saved in `localStorage` for the current browser and site. Each browser starts with its own copy of the sample collection. The original server-based login and registration screens are outside the front-end scope.

## Course topics demonstrated

| Topic | Where to find it |
| --- | --- |
| Timers | `app.js` delays search briefly while the user types and clears old notification timers. |
| Event listeners | `app.js` uses `addEventListener`, event delegation for movie actions, and `preventDefault` on form submission. |
| Error handling | `app.js` catches storage read and write errors. The collection remains usable when stored data cannot be read. |
| Custom validation | `movie-library.js` checks all eight fields and duplicate titles. `app.js` displays errors under their fields and updates them during editing. |
| Objects and classes | The `Movie` class describes catalog entries. |
| Array methods | `map` renders choices and records, `filter` searches and deletes records, `find` locates a movie, and `reduce` calculates ratings and genre counts. |
| Browser storage | The JavaScript library saves and restores the collection using JSON and `localStorage`. |

[JavaScript (Advanced) reference notes](https://dotnethow.net/full-stack-path/javascript-advanced/reference)

## Source files

- `index.html` contains the catalog, management view, and dialogs.
- `styles.css` is the shared CSS library for layouts, forms, buttons, cards, and tables.
- `movie-library.js` handles validation, search, statistics, and persistence.
- `app.js` connects the HTML to the library.
- `movies.js` contains the original sample catalog.

## Deployment

Publish this directory to Cloudflare Pages as a static site. Use the project root as the output directory with no build command.
