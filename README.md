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


## v13 update
- Removed the Weekly History section from the app.
- Previous Days remains the single source for viewing and editing completed days.
- Existing saved data and New Day behavior are preserved.
\n\n## v14\n- Fixed Start New Week button.\n- Added weekly weigh-ins and 10% milestone tracking.\n
## v15 fix
- Weekly Weigh-In progress now uses the most recent weigh-in date and shows pounds lost, remaining pounds, milestone count, and progress to the next 10% milestone.
- Saving or editing the newest weigh-in now automatically recalculates the Daily POINTS Target.
- On app load, the current Daily POINTS range is synchronized to the most recent saved weigh-in.

## v16 critical repair
- Fixed a JavaScript syntax error introduced in v14/v15 migration code that prevented the weigh-in and daily target update code from running.
- Saving a later weigh-in now updates weight-loss progress and the current Daily POINTS range.


## v17 critical fix
- Removed a remaining JavaScript syntax error that prevented the app script from running.
- Daily POINTS Target now synchronizes to the newest saved weigh-in on every refresh/update.
- Weight-loss progress now renders from the saved weigh-in history.
- Service-worker cache was corrected from the stale v11 cache name to v17 and now fetches fresh files before falling back to cache.
- JavaScript was syntax-checked with Node before packaging.

## v18 cache reset / tracker repair
- Removed the old offline service-worker caching layer that could keep the installed app stuck on an older version.
- Added a visible v18 marker in the app header.
- Changed the installed-app start URL to index.html?v=18.
- Daily POINTS calculation now writes directly to both the Daily Target result and Today's Tracker.
- Weekly weigh-ins still preserve localStorage data and update the latest weight, progress, and daily range.
