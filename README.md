# UB AI Showcase demos

## Bulls on the Loose

A colorful, one-button browser runner. Victor E. Bull tries to cross campus by jumping over Canada geese and poop. Short rounds and quick restarts let visitors take turns at the table.

The [reusable prompt](prompts/bulls-on-the-loose.txt) is the complete build brief. Copy the whole file into a coding assistant with an empty working folder. It asks the assistant to create `game/index.html`, which opens directly in a browser and works offline once generated.

This repo contains the prompt, demo plan, and a sample screenshot. Reusing the prompt should recreate the concept and features; artwork, code, and difficulty will vary between runs.

### Sample result

One generated version, shown as an example. The screenshot isn't required to use the prompt.

![Bulls on the Loose showing Victor E. Bull, a goose, and a game-over message after stepping in poop.](samples/bulls-on-the-loose.png)

## First version

- One action: jump. Ground geese and poop are the hazards.
- Original drawn mascot and scenery, with UB blue and white leading the design.
- Gradually increasing speed, distance score, and a best score saved in the visitor's browser.
- Keyboard and touch controls, pause, and a fast restart.
- One HTML file with no installs or runtime network access.

Keep ducking, flying geese, sound, and power-ups out of the first build. They're useful changes to demonstrate once the basic game works.

## Table demo plan

1. Before the event, run the prompt in a fresh folder. Play the result on a laptop and phone-sized viewport, and check that it works offline. Save a known-good copy separately as a fallback.
2. At the table, show the prompt and explain the goal: describe a small game, let AI build it, then test what it made. Start a fresh generation while visitors play the saved copy. Generation time will vary.
3. Open the new game and let a visitor try a round. Show how you check the controls, collisions, and difficulty instead of assuming the generated code works.
4. Ask the visitor for one change. Apply it, reload, and try it together. Keep the original copy available for the next visitor.

Possible follow-up prompts, used one at a time:

> Add an Easy mode with a slower speed cap and wider obstacle spacing. Keep the existing mode. Let players choose before starting, and track a separate best score for each mode.

> Add an optional synthesized honk when a goose ends a run. Include a labeled sound toggle, default it off, and only initialize audio after a user gesture. Keep the game self-contained and playable offline.

> Add a "Goose patrol" practice mode. Show the collision boxes and allow a slower game speed so we can see how jumping and collisions work. Keep practice scores out of the best-score record.

## Reference notes

- The [UB AI Showcase announcement](https://www.buffalo.edu/ubit/news/article.host.html/content/shared/www/ubit/news/2026/ubit-new-AI-Showcase.detail.html) lists November 4, 2026, 10 a.m. to 3 p.m., in the Student Union, with drop-in demonstrations including AI for Developers.
- UB identifies its blue bull mascot as [Victor E. Bull](https://www.buffalo.edu/trueblue/our-stories.host.html/content/shared/www/trueblue/articles/victor-history.detail.html).
- Colors follow the [UB palette](https://www.buffalo.edu/brand/creative/color/color-palette.html), including UB Blue `#005bbb` and white `#ffffff`.
- The campus goose problem is the participant's premise for the joke, not a measured population claim. The prompt uses the species name "Canada geese."

References checked October 30, 2026.
