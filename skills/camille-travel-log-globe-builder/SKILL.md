# Camille Travel Log Globe Builder

## What It Does

Turns a plain list of countries someone has visited into a shareable travel log. For each country it drafts a short trip summary, links to the itinerary the traveler wrote for that trip, collects their tips and recommendations, and produces a country-code list that a map or globe view can shade in.

## When To Use It

Use this skill when a learner wants to practice describing a travel scrapbook workflow. It fits when someone has a scattered pile of trip notes and wants them organized into one log that friends can browse country by country, with a visual sense of where they have been.

## Inputs

- A fictional list of countries visited, with the year of each trip.
- Optional links or file names for the itinerary written for each country.
- Tips and recommendations the traveler wants to pass along, such as a favorite neighborhood or a dish to try.
- A preferred sort order for the log, such as newest trip first or alphabetical by country.
- Whether the visual summary should be a globe or a flat world map.

## Output

A travel log with one section per country, each containing the trip year, a two-sentence summary, the itinerary link, and a short tips list. Above the sections it adds a count of countries visited and a list of ISO country codes ready to hand to a globe or map view. It closes with a list of any countries that are missing an itinerary link, so the traveler knows what to fill in next.

## Example Prompt

```text
Here is my made-up travel list: Iceland in 2021, Peru in 2022, and Vietnam in 2024.
I have itinerary notes for Iceland and Peru but not Vietnam yet. For tips I want to
mention a hot spring near the ring road, a bakery in Cusco, and a night market in
Hanoi. Build my travel log sorted newest first and give me the country codes for a
globe view.
```

## Safety Notes

Use invented countries, trips, and recommendations only. Do not include real passport or visa details, boarding passes, home or hotel addresses, booking confirmation numbers, frequent flyer accounts, payment details, or other travelers' names and locations without their consent. Keep the log fictional and safe to publish in a public repository.
