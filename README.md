# Foodie — React Native Recipe App

Foodie is a local recipe collection built with React Native and Expo. Browse ten horizontally scrollable food categories, read recipe details, save favorites, and manage your own recipes with photos. Personal recipes and favorites persist on the device with AsyncStorage.

## Run locally

This project uses **Expo SDK 54**, React Native 0.81.5 and React 19.1.

```sh
npm install
npm start
```

Open the project in an Expo Go client compatible with SDK 54, or use a matching development build. For a browser preview, run `npm run web`.

## Import into Expo Snack

1. Open [Expo Snack](https://snack.expo.dev).
2. Choose **Import Git Repository** and enter `https://github.com/yaroslavsts/foodie-react-native-course-project`.
3. Use an **SDK 54** runtime and allow the dependencies in `package.json` to install.
4. Run the preview and open `App.js`. Bundled illustrations are in `assets/` and sample recipes are in `recipes.js`.

The live Snack import could not be verified because the Snack site failed DNS resolution in the test browser. Local Expo builds and the iOS simulator flow were verified; see `VERIFICATION.txt`.

## Review walkthrough

1. Swipe the category strip horizontally. It contains Breakfast, Lunch, Dinner, Salads, Soups, Pasta, Desserts, Snacks, Vegan and Drinks, plus All, Favorites and My Food.
2. Tap a category to filter the feed. Open a recipe to see its image, ingredients, numbered instructions, preparation time, servings, calories and difficulty.
3. Tap the heart to favorite a recipe. Use **Back**, then **Favorites**, to find it. Tap the heart again to remove it.
4. Open **My Food → Add New Recipe**. Enter the name, ingredients and instructions, one item per line. Choose an image with **Upload Image**, then **Save Recipe**. Time, servings, calories, category and difficulty can also be changed.
5. The recipe appears in **My Recipes**. Open it to inspect the details, or use **Edit** to update it. **Delete** asks for confirmation; Cancel keeps the recipe.
6. Restart the app to verify that recipes and favorites persist.

The app uses bundled illustrations and local storage, with no account or backend required. The sample calorie figures are illustrative. Image selection uses the system photo picker; selected photo data is retained with the personal recipe.

## Project files

- `App.js`: screens, navigation, recipe form, filtering and persistence.
- `recipes.js`: ten sample recipes, one per category.
- `assets/`: bundled recipe illustrations.
- `app.json`: Expo and image-picker configuration.

Reference: [Expo SDK 54](https://docs.expo.dev/versions/v54.0.0/), [Expo ImagePicker](https://docs.expo.dev/versions/v54.0.0/sdk/imagepicker/).
