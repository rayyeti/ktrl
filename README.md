# KTRL — Kill Team Racing League Tracker

A mobile web app for running squig races at Kill Team events. Open it on any phone or tablet — no installation required.

---

## What is this?

Kill Team Racing League is a side event format for Warhammer 40,000: Kill Team, where players race small models (squigs, pets, helper creatures) around a track. This app helps the Tournament Organiser (TO) run the event smoothly — handling turn order, random events, and recording results.

---

## The two pages

**TRACKER** — used during a race  
**STANDINGS** — shows the cumulative league leaderboard

---

## Before the race

### Set the event name
Tap the event name field next to the KTRL logo and type the name of the event or heat (e.g. "GT Round 1"). This gets recorded with the results.

### Add racers
Tap **+ ADD RACER** to add a card for each player. For each racer, fill in:
- **Name** — the name of their model (e.g. "Fizzul")
- **@discord** — the player's Discord handle, for league tracking
- **Archetype** — select from the dropdown (Speedster, Balanced, Bruiser, Flyer). This auto-fills their base stats for reference.

---

## Running a race

### Roll Initiative
At the start of each round, tap **⚄ ROLL INITIATIVE**. The app rolls a d6 for each active racer, resolves any ties automatically, and sorts the cards into turn order. The number on the left of each card shows when that racer activates this round.

### Activation cycle
Each racer card has a cycle button showing their activation state:
- **READY** — waiting to take their turn
- **▶ ACTIVE** — currently taking their turn
- **✓ DONE** — finished for this round

Tap the button to advance through the states. Roll Initiative at the start of each new round to reset everyone to READY and re-randomise the order.

### Finishing the race
When a model crosses the finish line, tap its **FINISH** button. The button turns into a checkered pattern and the card shows their finishing position (1st, 2nd, 3rd...). If you tap it by mistake, tap again to undo — positions will adjust automatically.

---

## Reference tools

### ⚑ REF
Opens a quick-reference sheet with:
- Archetype stats (wounds, APL, movement)
- The Jostle effect table (what happens when models collide)
- All condition definitions
- A link to the full rules (https://docs.google.com/document/d/12b_6x96np8t7k9IgRh1B0_l-K7mdzriTY9jPnyveKJs/edit?usp=sharing)

### ⬡ FLOOR PLATE
During a race, the track has hidden floor plate tokens. When a model lands on one, the TO uses this panel to resolve the effect:

1. Set the **position** of the model that triggered it (1st, 2nd, 3rd...)
2. Tap **⚄ ROLL** — the app rolls a die, applies a bonus based on position (models further back get more powerful effects, like Mario Kart), and displays the result with full flavor text and instructions
3. Read the effect aloud and resolve it on the table

**Mad Bot Mode** (the HAL eye toggle at the top of the panel) switches to an alternate, wider pool of more unpredictable, modestly more unhinged effects brought to you by Claude.

---

## After the race

Once every racer has finished, the **SUBMIT RESULTS** button at the bottom activates. Tap it to send the results to the league Google Sheet. Results include each racer's finishing position, points, handler, and archetype.

Points are awarded as follows:

| Place | Points |
|-------|--------|
| 1st | 6 |
| 2nd | 4 |
| 3rd | 3 |
| 4th | 2 |
| 5th | 1 |
| 6th | 0 |

Tap **RESET** (double-tap to confirm) to clear the tracker for the next race. The event name and Sheets URL are preserved.

---

## Standings

The **STANDINGS** page pulls live data from the league Google Sheet and shows cumulative rankings by handler and by racer, including total points, race count, wins, podiums, and points-per-race average. Tap **↻ REFRESH** to update.

---

## Setup (for the TO)

Example boards (long side half-width kill team board, 11x30")
<img width="4550" height="2149" alt="IMG_4378" src="https://github.com/user-attachments/assets/f1d1923e-4414-40c1-9326-580fb658a00d" />
<img width="5380" height="2683" alt="IMG_4237" src="https://github.com/user-attachments/assets/a48ca27c-3279-4899-a664-2798b2e06ba8" />
