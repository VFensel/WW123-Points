# Classic WW POINTS Calculator — v6

Updates:
- Replaces the prior Basic Food List with the full requested food reference list.
- Organizes the dropdown into Meat/Poultry/Fish, Eggs/Dairy, Bread/Grains/Starches, Vegetables, Fruit, Nuts/Fats/Condiments, and Treats/Extras.
- Displays serving size and POINTS directly in the dropdown.
- For entries listed as a POINTS range, the higher value is entered automatically for conservative tracking.
- Keeps the v5 favorite-food fix: tapping a saved favorite adds it directly to today’s Food Log.
- Keeps Daily POINTS Target, Food Log, Previous Days, sharing, and saved browser data.
- Cache bumped to v6 for installed-app updates.


## v7 update
- Fixed **New Day** so it closes the current day, saves the food entries to Previous Days, and clears Today's Tracker/Food Log for a fresh day.
- Added **Edit** to every item in Today's Food Log so the food name or POINTS value can be corrected without deleting and re-entering it.
- Bumped the service-worker cache to v7 so installed apps receive the update.

## v8 update
- Previous Days can now be edited.
- Add a missed food item directly to yesterday or another prior day.
- Edit or remove individual foods from a prior day.
- Prior-day totals recalculate automatically, including matching history/bank adjustments when available.


## v9 Restaurant POINTS update
- Added Restaurant POINTS for McDonald’s, Wendy’s, Taco Bell, Arby’s, KFC, Subway, Pizza Hut, Culver’s, Burger King and Dairy Queen.
- Restaurant search, quantity selector, combined classic-POINTS calculation before rounding, and Add Today button.
- Values are calculated with the classic calories/fat/fiber formula from published nutrition references; restaurant recipes can change.


## v10 update
- Moved the Share App button to the bottom of the app page.


## v11 layout update
- Removed the empty Share This App card from the top.
- Added a purple app header with the app icon and subtitle.
- Reorganized the page into cleaner rounded cards.
- Favorite Foods, Previous Days, Restaurant POINTS, Weekly History, Historical Daily Range, and Important are now compact expandable sections.
- Kept Food Calculator, Daily Target, Today's Tracker, and Food Log immediately accessible.
- Moved Share This App to a bordered button at the bottom.
- Added a fixed bottom navigation bar for Calculator, Food Log, Favorites, and History.
- Preserved all v10 tracking, editing, restaurant, and previous-day functionality.


## v12 history fix
- Fixed Weekly History so it uses the same saved-day data as Previous Days.
- Weekly History now shows the same completed days and food entries instead of relying only on the older summary-only history array.
- Weekly POINTS bank and activity/net information are still shown when available.
