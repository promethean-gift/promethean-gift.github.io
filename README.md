# promethean-gift.github.io

Bootstrap github.io website for Promethean Gift test website

## Website development

To run locally:
```
git clone https://github.com/promethean-gift/promethean-gift.github.io.git
cd cyverse-gis.github.io
npm install
npm run serve
```

Managing the navbar Edit views/Navbar/pages.json to change the links at the top of the page.

Controllers, custom views Most pages should be able to just use `controllers/VanillaController.js`, that manages the navbar at the top and the footer at the bottom (`<header>` and `<footer>` tags are needed in the page's HTML for these to work).

The custom views in place (such as the header and footer) use the uki.js MVC framework; using the framework is optional, or feel free to include your own.

npm libraries Feel free to `npm install --save` any libraries that you need, but you will also need to edit .gitignore to specifically include the files that you actually link to inside node_modules (so that we don't end up committing the whole directory structure).
