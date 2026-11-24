# Menu Board

Plain HTML, CSS and JavaScript. No libraries.

## Run it
`fetch()` can't read local files when a page is opened by double-clicking, so serve the folder:

- VS Code: install "Live Server", right-click index.html, "Open with Live Server"
- or in this folder run: `python -m http.server 8000` and open http://localhost:8000

## Structure
index.html                      page shell, loads all CSS and JS
css/base.css                    colours, reset, focus styles
css/layout.css                  top bar and page width
css/components/*.css            one stylesheet per component
js/utils.js                     h() element builder, rupees()
js/api.js                       fetchRestaurants() – set API_URL here
js/components/*.js              Message, Chip, SearchBar, FoodCard, RestaurantSection
js/app.js                       state, filtering, rendering
data/menu.json                  sample restaurants and menus

## Add a restaurant
Add an object to data/menu.json. A new section and filter chip appear automatically.
