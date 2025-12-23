---
{"dg-publish":true,"permalink":"/notes/reading-notes/validating-your-game-design/","tags":["reading_notes/video","gamedev"]}
---

My notes on the talk [Validating Your Game Design: Ways to confirm the potential of your game idea before launch](https://www.youtube.com/watch?v=3Sfa8PbEE3U) by [Oscar Clark](https://bsky.app/profile/athanateus.bsky.social)

Presentation mostly Targeted to Live games
Some questionable design patterns, in [[Notes/reading notes/Validating Your Game Design#Mechanics\|Validating Your Game Design#Mechanics]] for example
# Direction
## What success looks like?
Pick 3, and put number on them! => KPI/Metrics
It can be:
- Communicate Ideas
- Looking for Inner Truth
- Pure Gameplay
- Love for Genre
- Professional Accolade
- Need to innovate
- Financial success
- Market Opportunity
## What are you making
- Toy?
	- Short term revenue model
- Long term investment game?
	- Game as a Service?
## Understand you audience
3 Personas
- Persona 1 - HOW (Mechanics)
	- In love with core mechanics
	- Will continue playing if the game was only the core mechanics
- Persona 2 - WHAT (Context)
	- need a sense a purpose to continue playing
- Persona 3 - WHY (metagame)
	- Social component
	- Livestyle / Daily routine

=> Targetable audience
Everything needs to be build in the design
## Design
### Loops
#### Mechanics
Think about the emotional journey of the player
1. Start condition
	Does the player enter the game in a relaxed state? Does he enter the game with anticipation
2. Challenge
	Are we introducing a sense of tension?
3. Resolution
	Move away from anticipation toward FOMO
1. Reward
	=> Relief, but without satisfying the player fully so he continue to engage
	Keep player in the FOMO, even when we give the reward
#### Context
#### Metagame
Not the game
What happen outside of the game
### Extensible interaction
Interaction that can
- Show off my skill
- Encourage my brain to work
- Be enhanced by powerups
=> Tap into to give player a sense of autonomy/control
### Art/IP Fit
Is the art suitable for the IP
### Game economy
This encompasses everything, like  
Gold / Player Time / XP / Consumables / ...
Think about how they all interact together and where does your business model fits in
# Data
## Where do we get data?
### User testing / Qualitative testing
Online playtesting platform : https://antidote.gg/
Great to recruit 5/10 people.

Have some telemetry ready to understand what path do they take / where they are stuck.

Ask 3 Questions
- Did they enjoy playing the game -> They will lie
- Would they play the game again -> They will lie again
- Would they recommend to a friend -> They already lied twice, they are much likely to give an honest answer here
### Attribution partner
https://steamdatasuite.com/
When I run a marketing campaign, where does the player comes from?
### In game data
It's increasingly difficult to extract raw data from game platform, so we need to back data gathering into the game -> ship to an Object Storage and observe with another software (Dataiku :))

Example of data
1. Event trigger
	With context, anonymized of course
	2. Level start
	3. Level end
	4. Shooting action
	5. End of a match
		With context, so we can mesure a Win / Loss ratio

### Market data
vginsight, steamspy, steamdb
## What do we do with the data
=> Average of 10 games in the subgenre
=> Create revenue possibility
⚠️ It's not forecast, it's what success can look like

Top down analysis with Market data:
What the market is looking like?
What the growth is looking like?
=> Create KPI to use to mesure our likelihood of success

Bottom up analysis
- Make assumption on KPI
- What revenue can the game make if those KPI are true

Build Data targets
- Optimal
- Good
- Mid
- Fail
=> Can be used to make tests:
- share trailer with real targeting but small audience
- with expected KPI
	- Cost per click / Cost per install
- See in which target we land

Example Indicators
- Cost per click / Cost per install
- Retention
- ROAS: Return on Advertising Spend
- ARPDAU: Average Revenu Per Daily Active User

# Game report
Rate every next points with N/A, ISSUES, PARTLY, MOSTLY, GOOD
Detail every category by answering the questions:
- What this does well
- Recommendations
- Questions and potentials risks
## Game design
Compelling core mechanic
Gameplay is extensible
Sense of purpose and progression
Play fits lifestyle & Mode of use
Compelling social experience
## Monetization Design
Focus on player utility
Monetization fits platform/genre
Good use of hybrid monetization
Reasons for repeat purchase
Purchase experience is satisfying
