# Data

We use FanGraphs prospect rankings and the players' later MLB WAR to test whether the evaluations systematically misvalue players. We look at three possible sources of bias: developmental origin and age, physical build, and raw tools versus game skills.
 
**Uncleaned Data:** `Prospect Rankings Data (Uncleaned).csv`. It holds FanGraphs prospect rankings (one row per player per ranking year) joined with MLB WAR by season, 2020–2026.
 
**Unit of observation (after cleaning):** one row per prospect. Each row uses the prospect's most recent ranking year.

**Cleaned Data:** 

## Codebook

- **Name**: Player name.
- **Year**: Year of the player's most recent FanGraphs ranking. Range: 2020–2023.
- **Org**: MLB organization at the time of ranking. Values: team abbreviations (e.g., KCR, SEA).
- **Rank**: Overall prospect rank. Range: 1–100+ (1 = best).
- **Pos**: Listed position. Values: C, 1B, 2B, 3B, SS, LF, CF, RF, DH, SP, RHP, LHP, MIRP, SIRP.
- **Pos Group**: Position grouped for comparison. Values: C, IF, OF, P.
- **Age**: Age at time of ranking. Units: years.
- **Height**: Player height. Units: inches.
- **Weight**: Player weight. Units: pounds.
- **Height Build / Weight Build**: Height or weight compared to others at the same position (more than 1 standard deviation from the position average counts as atypical). Values: Short/Typical/Tall and Light/Typical/Heavy.
- **Signed.From**: School, college, or country the player signed from. Values: text.
- **Sign.Mkt**: Market the player signed in. Values: e.g., J2, Intl15, draft.
- **Background**: Developmental origin, based on Signed.From and Sign.Mkt. Values: High School, College, International, Unknown.
- **Bonus**: Signing bonus. Units: US dollars.
- **Risk**: FanGraphs' risk that the player doesn't reach his FV. Values: Low, Med, High.
- **FV**: FanGraphs Future Value grade. Range: 20–80 (scouting scale).
- **Tool grades (Hit, Game, Raw, Spd, Fld, FB, SL, CB, CH, CMD)**: Future scouting grades for hitting, game power, raw power, speed, fielding, fastball, slider, curveball, changeup, and command. Range: 20–80.
- **Max.EV**: Maximum exit velocity (for hitter). Units: mph.
- **Hard.Hit**: Hard-hit rate (for hitter). Range: 0–1 (proportion of batted balls).
- **Tops**: Maximum Fastball velocity. Units: mph.
- **RPM.Break**: Spin rate of breaking ball. Units: rpm.
- **2020 WAR – 2026 WAR**: Wins Above Replacement in each MLB season (0 if the player didn't play). Units: WAR.
- **Total WAR**: Sum of all season WAR. Units: WAR.
- **Seasons Played**: Number of seasons with nonzero WAR. Range: 0–7.
- **Average WAR**: Total WAR ÷ Seasons Played (0 if never reached MLB). Units: WAR per season.
