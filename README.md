# Recipes

Healthy, very simple lunches. Each recipe is one markdown file in `recipes/`, with structured info in the frontmatter and the instructions below it.

Swipe through the menu at **https://spyqs.github.io/food-recipes/**. Any recipe pushed to `main` shows up there automatically.

## What gets tracked

- **Nutrition:** calories, protein and fiber, plus carbs and fat
- **Simplicity:** difficulty, subjective effort (1 to 5), active and total time, number of steps and ingredients
- **Flavor:** a 1 to 5 rating, added after eating

## Adding a recipe

Copy `TEMPLATE.md` to `recipes/<recipe-name>.md` and fill it in, or describe the meal to Claude and have it write the file. Photos go in `images/`, named after the recipe.

## Asking Claude for help

- "Plan five lunches for next week and give me a shopping list."
- "Which recipes have the most protein for under 500 calories?"
- "What can I make in under 15 minutes with what's in my freezer?"

`CLAUDE.md` tells Claude how to work with these files.
