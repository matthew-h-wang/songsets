An inventory-style webapp (Node/Express/EJS/MySQL) for managing your bands' setlists.
Currently hosted at [songsets.up.railway.app/](https://songsets.up.railway.app/).

## Features:
- Auth0 powered login
- Users can create and join bands, allowing collaboration with different roles (owner, core, readonly).
- Each band maintains their own library of songs and setlists of those songs
- Easily add, delete, and reorder songs within setlists, plus add performance notes for each song in the list.
- See a song's history of use across setlists.
- Songs can be searched/sorted by title, tags, last date played, etc. 
- Setlists can be searched/sorted by name, date, last updated, songs, etc.
- Songs and setlists can be archived (and unarchived), maintaining complete records while reducing clutter for future setlists.

## Notable Libraries used:
- [mysql2](https://www.npmjs.com/package/mysql2) 
- [MaterializeCSS](https://materializecss.com/)
- [EJS](https://ejs.co/)
- [List.js](https://listjs.com/docs/)
- [SortableJS](http://sortablejs.github.io/Sortable/)

### Big TODOs:
- Server-side form validation
- API and route testing
- (More) Client-Side-Rendering (React/NextJS)?
- Utilize ORM (Prisma)
    - pub/sub for concurrent (collaborative) set/song editing

### Small TODOs:
- Patch out use of EJS on browser side (may require proper CSR framework)
- Add song page's list of sets to include performance notes of that song (again, more CSR work)
- Better HTTP error codes + nicer looking 404 pages (natural redirects?)
- Update user management list to be more like the other lists
- Refactor route handlers into routes/controllers?
