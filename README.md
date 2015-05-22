# NBA "Last Two Minutes" officiating report analysis

## Resources:
- [official release](http://www.nba.com/2015/news/02/27/officating-reports-official-release/)
- [report archive](http://official.nba.com/nba-last-two-minute-reports-archive/)
- [point of emphasis: traveling](http://official.nba.com/wp-content/uploads/sites/4/2015/03/021815-2014-15_POE_MEMO_8-PERFORMANCE_UPDATE_AND_TRAVEL_CALLS.pdf)
- [decline home court advantage](http://espn.go.com/nba/story/_/id/12241619/home-court-advantage-decline)

## Output key
From the NBA:
*"The plays assessed include all calls (whistles) and notable non-calls. Notable non-calls will generally be defined as material plays directly related to the outcome of a possession."*

- **quarter**: The quarter of the play. Uses Q5+ for OTs.
- **time**: Time of the play (minute:second:tenth of second).
- **call_category**: The more general bucket of call that was made.
- **call_type**: The specific type of call that was made.
- **committing_player**: The player who committed the infraction. 
- **disadvantaged_player**: The player who the infraction was committed against.
- **committing_team**: The team who committed the infraction. 
- **disadvantaged_team**: The team who the infraction was committed against.
- **decision**: The outcome of the officials post-game review (CC: correct call, IC: Incorrect call, CNC: Correct non-call, INC: Incorrect non-call).
- **indirect**: From the NBA *"Calls that are indirectly related to the outcome (e.g., a non-call on contact away from the play) and/or plays that are only observable with the help of a stop-watch, zoom or other technical support, but have some merit in reporting".*
- **comment**: The description of the play that occured.
- **flag**: If the data seems like it might not follow the proper structure it is flagged for manual evaluation.
- **date**: The date of the game.
- **away**: Away team.
- **home**: Home team.
- **winner**: Winner of the contest.
- **game**: The way to identify a specific game (matchup + date).
- **video**: Video link to the play.
- **ref_1**: Referee.
- **ref_2**: Referee.
- **ref_3**: Referee.
- **game_info**: Url to full game recap (article, box score, etc).
- **source**: Url to pdf.

## Questions
- How often do refs "swallow the whistle" (miss a call) in a close games?
- Do referees make more decisions in favor of the home team?
- How often does an incorrect call **directly** lead to points?
- Do the incorrect calls tend to make the game closer or further?
- What calls are referees getting wrong most often?
- Is there any star treatment?
- Do certain teams benefit from referee decisions?
- When are the wrong calls made?