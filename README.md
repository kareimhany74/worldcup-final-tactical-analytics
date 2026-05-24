# 2022 FIFA World Cup Final Tactical Analytics: Argentina vs. France

An advanced Sports Data Science project that performs a deep tactical and statistical event-data analysis of the legendary 2022 World Cup Final. Utilizing official open-source tracking/event data from **StatsBomb**, this project reconstructs the match events to uncover spatial patterns, player impacts, and team dynamics.

---

## Project Overview
The 2022 World Cup Final between Argentina and France was arguably the greatest football match in history. This project moves beyond the basic scoreline to analyze the underlying data. By pulling high-fidelity event data, we map out expected goals (xG), team pressing intensities, defensive recoveries, and individual superstar performances (Lionel Messi vs. Kylian Mbappé).

## Technical Skills & Tools
* **Language:** Python
* **Environment:** Jupyter Notebook
* **Specialized Sports Analytics Libraries:** statsbombpy, mplsoccer
* **Core Data Science Libraries:** Pandas, NumPy, Matplotlib, Seaborn

---

## Data Pipeline & Methodology

### 1. Match Event Extraction & Identification
* Connected to StatsBomb API to isolate the 2022 World Cup Competition (`competition_id=43`, `season_id=106`).
* Programmatically filtered and extracted the exact Match ID for the Argentina vs. France final.

### 2. Shot Map & Expected Goals (xG) Visualization
* Plotted all match shots on a professional dark-themed soccer pitch.
* Sized individual shot markers dynamically based on their xG value (probability of scoring) to visually showcase the danger zones each team created.
* Isolated and highlighted the actual goal events for both sides.

### 3. Cumulative xG Timeline (The Match Flow)
* Built a step-chart tracking the chronological progression of Cumulative Expected Goals (xG) for both nations across regular and extra time.
* This chart illustrates the shifting momentum of the match, from Argentina's early dominance to France's dramatic comeback.

### 4. Spatial Heatmaps & Team Territory
* Cleaned and extracted 2D coordinates (`x, y`) from thousands of raw match events.
* Generated density heatmaps to analyze which areas of the pitch were heavily controlled or contested by each squad.

### 5. Superstar Head-to-Head: Messi vs. Mbappé
* **Lionel Messi Profile:** Formatted a detailed touch map, progressive carries, and successful pass networks showing how he dictated the play from deep channels.
* **Kylian Mbappé Profile:** Analyzed his clinical output, attacking efficiency, and shooting positions.

### 6. Modern Pressing & Defensive Metrics
* **The Engines (Pressure Events):** Aggregated and identified the top 5 high-intensity pressing players who broke up the opponent’s build-up play.
* **Ball Winners:** Analyzed combined defensive actions (Tackles, Interceptions, and Ball Recoveries) to pinpoint the defensive pillars of the match.
* **Shot Assists:** Isolated key passes that directly led to a shot, mapping out the main creative playmaker hubs.

---

## Repository Structure
```text
├── final world cup.ipynb         # Comprehensive Jupyter Notebook with all data extraction & plots
└── README.md                     # Advanced project documentation (This file)
