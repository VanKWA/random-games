# Random Games Kids POC v8

Ad-free static web app for phone-friendly kids games. Designed to run from GitHub Pages with no server and no login for players.

## Included tabs

- **Math**: generated connected math crossword puzzle
- **Other Games**: placeholder for future games
- **Draw**: finger/mouse drawing canvas with color picker, fill color, shape correction, local saving, and PNG download

## Math level progression

The math puzzle generates new connected crossword-style levels indefinitely. The level number keeps increasing; the rules get harder at milestones.

- Levels 1-5: + and - only, single-digit numbers
- Levels 6-10: + and - up to 20
- Levels 11-15: + and - up to 30
- Levels 16-19: simple multiplication, product under 20
- Levels 20-24: product under 20; addition/subtraction up to 30
- Levels 25-29: product under 30; addition/subtraction up to 40
- Levels 30-34: product under 30; addition/subtraction up to 40; division under 15, whole numbers only
- Levels 35-39: division under 20; product under 30; whole numbers only
- Levels 40-44: division under 20; product under 30; addition/subtraction up to 50
- Levels 45-49: addition/subtraction up to 100; product under 30; division under 20
- Levels 50+: balanced puzzles with 2 addition equations, 2 subtraction equations, 1 multiplication equation, and 1 division equation

## Rewards

- Auto-checks when every green box is filled
- Congratulations popup uses the selected player's name
- Confetti burst and sound effect on correct completion
- Stars based on time, mistakes, and boxes filled
- Bonus stars for beating best time, reducing mistakes, and beating previous record score
- Evaluation page tracks mistakes by operation and range

## Storage

Profiles, progress, mistake history, and drawings are saved locally in the browser using localStorage and a cookie mirror. There is no cloud database.

## Run locally

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## GitHub Pages

Upload `index.html` to the root of your GitHub repo and enable Pages from the `main` branch root folder.
