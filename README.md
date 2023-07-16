Problem Statement. Develop a recipe generator algorithm that takes into account user preferences and generates customized recipes based on those preferences.

Sub-Problems.
1. User Input.
   - Sub-Problem. A user with dietary restrictions may not be able to find recipes they can eat.
   - Sub-Solution. The recipe generator could prompt the user for their dietary restrictions and then filter the recipe database to only include recipes that are compatible with those restrictions.

2. Recipe Selection.
   - Sub-Problem. A user may not have time to cook a complicated recipe.
   - Sub-Solution. The recipe generator could filter the recipe database to only include recipes that are relatively easy to make.

3. Recipe Information.
   - Sub-Problem. A user may be unskilled in cooking or not able to read the instructions for a recipe because they are in a foreign 
 language.
   - Sub-Solution. The recipe generator could translate the instructions for the recipe into the user's preferred language.

Functions Necessary.

1. getting user preferences().
   - Function to prompt the user for their dietary restrictions and store their preferences.

2. filtering recipes by restrictions(preferences, recipe database)
   - Function to filter the recipe database based on the user's dietary restrictions/preferences.
   - Input: preferences (user's dietary restrictions/preferences), recipe database
   - Output. filtered recipes (recipes compatible with the user's preferences)

3. filtering recipes by complexity(time available, recipe database).
   - Function to filter the recipe database based on the user's available time.
   - Input. time available (user's available time), recipe database
   - Output. filtered recipes (recipes that are relatively easy to make within the given time)

4. translating recipe(recipe, target language):
   - Function to translate the recipe instructions into the user's preferred language.
   - Input. recipe (a single recipe with instructions), target language
   - Output. translated recipe (recipe with translated instructions)

5. generating customized recipes(preferences, time available, recipe database, target language)
   - The main function that integrates all the sub-solutions and generates customized recipes.
   - Input. preferences (user's dietary restrictions/preferences), time available (user's available time), recipe database, target language
   - Output. customized recipes (filtered and translated recipes based on user preferences)

Defining of variables
1. getting user preferences()
   - preferences: List to store the user's dietary restrictions/preferences.
   - user input: String to store the user's input for each dietary restriction/preference.

2. filtering recipes by restrictions(preferences, recipe database)
   - preferences: List of dietary restrictions/preferences provided by the user.
   - recipe database: List or database structure storing recipes.
   - filtered recipes: List to store recipes that are compatible with the user's preferences.

3. filtering recipes by complexity(time available, recipe database)
   - time available: Numeric value representing the user's available time.
   - recipe database: List or database structure storing recipes.
   - filtered recipes: List to store recipes that can be prepared within the given time.

4. translating recipe(recipe, target language)
   - recipe: Recipe object or data structure representing a single recipe.
   - target language: String representing the user's preferred language.
   - translated recipe: Recipe object or data structure with translated instructions.

5. generating customized recipes(preferences, time available, recipe database, target language)
   - preferences: List of dietary restrictions/preferences provided by the user.
   - time available: Numeric value representing the user's available time.
   - recipe database: List or database structure storing recipes.
   - target language: String representing the user's preferred language.
   - filtered by restrictions: List to store recipes filtered based on dietary restrictions.
   - filtered by complexity: List to store recipes filtered based on time availability.
   - customized recipes: List to store the final customized recipes.


