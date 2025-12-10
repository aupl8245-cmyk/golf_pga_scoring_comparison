# golf_pga_scoring_comparison
PGA Tour scoring averages project for 2016–2020 vs 2021–2025
---

## PGA Tour Scoring Analysis: 2016–2020 vs 2021–2025

[Click here to view my full scoring notebook](https://github.com/aupl8245-cmyk/golf_pga_scoring_comparison/blob/main/pga_scoring_analysis.ipynb)

I wanted to do something a little more personal for this project because golf is what I actually know. Instead of maps or species data, I built a full scoring analysis of the PGA Tour to see how course difficulty has shifted over the past decade. I compared scoring averages from 2016–2020 with the same tournaments from 2021–2025 and focused on ten events that stayed at the same course in both periods. That way the comparison is fair and the changes actually mean something.

### Events I analyzed
The Masters  
U.S. Open  
PGA Championship  
WM Phoenix Open  
Arnold Palmer Invitational  
THE PLAYERS  
Charles Schwab Challenge  
RBC Heritage  
John Deere Classic  
Sentry Tournament of Champions at Kapalua

These events give a mix of majors, flagship tournaments, and regular stops. They also cover a wide range of scoring styles, from major championship grind outs to resort style birdie fests.

### What I did

I pulled scoring averages from the PGA Tour scoring pages and built a pandas DataFrame with the following for every tournament and every year:

- Event  
- Year  
- Course  
- Par  
- Field scoring average  
- Winning score for context  

After loading everything in, I created a time period column to split the data into two windows: 2016–2020 and 2021–2025. I grouped the events by period and calculated mean scoring averages for each tournament. Then I ranked the tournaments from hardest to easiest and created bar charts to show the changes. My notebook walks through every step in the same workflow I used for my Orca and Gila projects. It is fully reproducible.

### What I found

The scoring barely changes at the Tour level. The overall average moves from about 71.02 to 70.95. That is basically nothing. So the sport is not suddenly way easier or harder.

But the events themselves tell a different story.

**The U.S. Open is still the hardest event by far.** The average score sits above 72 in both windows. It is the only tournament that regularly plays over par. Nothing else comes close.

**Kapalua is still the easiest.** It remains the purest birdie course on the Tour with scoring well below par in both periods. The gap between Kapalua and the U.S. Open is more than six shots per round.

**Majors as a group stay tougher than anything else.** They consistently average above the regular events and flagship tournaments. That makes sense when you look at course setups, weather, and field strength.

**A few events did change.**  
The Arnold Palmer Invitational and THE PLAYERS got slightly harder. Phoenix, John Deere, and the PGA Championship stayed almost identical. Harbour Town and Colonial softened a little. None of the shifts are huge but they do show how course changes and weather can nudge difficulty.

### Figures Included

**Figure 1:** Bar chart comparing field scoring averages for all ten events across both time periods.  
**Figure 2:** Difficulty shift chart showing which events got easier or harder between 2016–2020 and 2021–2025.

These figures make it clear that scoring patterns are stable overall, but individual events still have year to year swings based on wind, course changes, and how aggressively the Tour sets things up.

### Main takeaway

Golf does not change as fast as people think. Equipment, distance, and course design are always part of the conversation, but when you break the numbers down, the Tour basically holds the same difficulty identity year after year. Majors stay majors. Resort courses stay resort courses. The only big outlier is the U.S. Open, which continues to live in its own tier of difficulty.

This project let me take the same analysis skills from my earlier assignments and apply them to something I actually care about. It also made it easier to understand how to clean, organize, and compare multi-year sports data with pandas and build clear visuals that show the patterns.

