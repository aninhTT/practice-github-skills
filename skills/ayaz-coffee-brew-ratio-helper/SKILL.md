# Ayaz Coffee Brew Ratio Helper

## What It Does

Works out how much coffee and water to use for a given brew method and number of cups. It converts a
coffee-to-water ratio into gram and milliliter amounts, then lays out the pour steps in order with
rough timings.

## When To Use It

Use this skill when scaling a brew up or down for a made-up number of guests, or when switching
between brew methods and the usual scoop-and-hope approach stops working. It is meant for practicing
how a small unit-conversion helper gets described, not for tuning a real cafe menu.

## Inputs

- The brew method (pour over, french press, moka pot, cold brew).
- How many cups to make, and roughly how big a cup is.
- A preferred ratio, such as 1:16, if there is one.
- Optional: grind size and whether the beans are a light or dark roast.

## Output

A short brew card listing the coffee dose in grams, the water volume in milliliters, the water
temperature, and a numbered pour schedule with timings. Ends with one suggestion for what to adjust
if the result tastes thin or bitter.

## Example Prompt

```text
I want to make pour over coffee for four imaginary guests using a 1:16 ratio, about 250 ml a cup.
Give me the coffee dose, the water amount, and a pour schedule.
```

## Safety Notes

All brew examples are invented for practice. Do not feed this skill real cafe recipes, supplier
pricing, private notes, employee or customer information, or anything copied from a workplace
document. Ratios here are a rough starting point for a fictional exercise, not tested guidance.
