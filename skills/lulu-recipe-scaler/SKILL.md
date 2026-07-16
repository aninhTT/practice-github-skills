# Lulu Recipe Scaler

## What It Does

Rescales a fictional recipe to a new number of servings. It adjusts each
ingredient amount proportionally, converts awkward fractions into friendly
measurements, and flags any ingredient that does not scale linearly (like
spices or leavening) so the cook can taste and adjust.

## When To Use It

Use this skill when a learner wants to practice describing a simple
proportional-math workflow with a made-up recipe, without relying on any real
cookbook, brand, or private family recipe.

## Inputs

- A fictional recipe name.
- The original number of servings.
- The target number of servings.
- A list of ingredients with amounts and units.
- Optional notes about ingredients that should not scale linearly.

## Output

A rescaled ingredient list at the target serving size, rounded to practical
measurements, plus a short list of "taste and adjust" callouts for anything
that does not scale cleanly.

## Example Prompt

```text
I have a fake recipe called "Garden Party Lemonade" that serves 4. Scale it to
serve 10. Ingredients: 2 lemons, 1 cup sugar, 4 cups water, 1 pinch salt.
```

## Safety Notes

Use invented recipes and amounts only. Do not include real proprietary recipes,
brand formulations, private family recipes, personal files, or any customer,
company, or otherwise sensitive information.
