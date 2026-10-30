# Recipe repo

The goal is to make healthy, very simple lunches easy. What matters:

- Nutrition, especially protein, fiber and calories
- Simplicity: difficulty, steps, time and number of ingredients
- Flavor

No numeric targets are set yet, so ask rather than assume one.

## Adding recipes

- Follow `TEMPLATE.md`. File names are kebab-case, in `recipes/`.
- Nutrition is per serving. Prefer label values, otherwise USDA data, and record where the numbers came from in `nutrition_source`.
- Round calories to the nearest 10 and grams to whole numbers.
- `effort` and `flavor` are the user's own ratings. Leave them as `null` until the user gives them, and never guess.
- `difficulty` is how much skill a recipe takes. `effort` is how much of a hassle it feels.
- Photos go in `images/` as JPEGs named after the recipe, at most 1600px. Strip GPS data first, since phone photos can carry a home location.

## Menus and shopping lists

- Read the frontmatter of every file in `recipes/` first, and only use recipes that exist unless asked for new ideas.
- Show each day's calories, protein and fiber, plus the weekly average.
- Scale ingredient amounts by how many times a recipe is used, combine duplicates, and group by `aisle`.
- Convert to what the store sells: whole bags and tins, and dried amounts for beans. Note any leftovers.
- List `prep_ahead` items separately as batch prep to do before the week starts.
