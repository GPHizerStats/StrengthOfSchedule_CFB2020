## StrengthOfSchedule_CFB2020
###### *A google-sheets centered project displaying multiple aspects of strength of schedule in 2020 FBS football.*

### General Overview

My first venture into a "large-scale" analytics project, this project revolves around implementing a *BCS Poll-style* ranking for srength of schedule (SoS) for all NCAA football teams as the 2020 season wore on. The primary stats I was concerned about for this project include:
- **Overall Record** ~ Ranked according to winning %, with ties being broken by total wins
- **Overall Strength of Schedule (SoS)** ~ Using the same formula used by the BCS Poll where:
  - Wins against FCS schools are not included in record/win % calculations, but losses are.
  - Opponent's Winning % (OWP) and Opponent's Opponent's Winning % (OOWP) are averaged, with OWP being weighted twice as heavily as OOWP using the following formula: $$SoS = \frac{(2*OWP) + OOWP}{3}$$
- **Strength of Victory (SoV)** ~ Shows a team's SoS, only including teams which they have beaten in the OWP and OOWP calculations.
- **Strength of Schedule Remaining (Rem)** ~ Shows a team's SoS, only including teams which they have not yet played in the OWP and OOWP calculations.

### Sheets Overview

This project was done entirely via Google Sheets, and it consists of 4 key pages/page types which were all interlocked. These include:
- ***Main Page*** ~ The number one page of concern, this Google Sheet housed all of our primary findings, including a page for the top 25 across the nation in each of our Big 4 stats, as well as conference standings page for each stat. The conferences on each standings page were color-coded according to their official conference RGB values.
- **NCAA Records Sheet** ~ This page was the heart of the backend for this project, and the only page that needed to be updated weekly. There is a tab for each conference contains the schedule for each FBS team in the nation, as well as a binary scale for whether the game was played and if it was won. All calculations were based off of the results on this page, and once it was set up, it only took roughly 15-20 minutes each Sundau afternoon to update the games played, won, and cancelled (due to covid)
- **Conference Record Books** ~ Each conference also had a sheet to house the standings and calculations for each team. The sheet has a tab for each team in the conference, which pulls the team's schedule and binary data directly from the records sheet. From there, our Big 4 stats and any supplementary stats for the team are calculated on their own page. Finally, each conference book begins with a standings page that displays and rates record, SoS, and more for each team in the conference.
- **Raw Rankings** ~ Another backend file, this sheet pulls the Big 4 Stats from each conference sheet and then sorts all teams across the nation accordingly, assisting in the transition to the main page.

### Closing Remarks

While there are many flaws in the BCS model for strength of schedule, i.e. not all 7-5 teams are created equal, it is a good attempt to create an unbiased, assumption free ranking. This was my first large project revolving around sports statistics, and it displays a strong grasp on using Google Sheets and linking multiple pages, while also attempting to help visualize the data being found.

### Sheet Links
#### Due to the nature of linked Google Sheets, it is easier to link all of the sheets/folders, as opposed to downloading them and uploading to Github.

 - **Main Page**: https://docs.google.com/spreadsheets/d/1TFNaKZUs05yHqpAbEhycWAupor434tHVXlxLYXdw2tA/edit?usp=sharing 
 - **NCAA Records Sheet**: https://docs.google.com/spreadsheets/d/1SBqRWZOO0jMbO_fimdFPSfS-m-AnYyFu9UG5i0bsveE/edit?usp=sharing
 - **Conference Record Books Folder**: https://drive.google.com/drive/folders/1u8vZ66ASIM2YRjIcESbWp8GTkZlWHhGi?usp=sharing
 - **Raw Rankings**: https://docs.google.com/spreadsheets/d/1e8PC9TLlhpTDVcv6PSAbb3va5SM1NvumBbNYcunqLe4/edit?usp=sharing
