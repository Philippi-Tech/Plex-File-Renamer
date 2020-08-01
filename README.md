# Plex-File-Renamer
Rename TV Episodes to follow Plex formatting using online databases

# Objective
Read a directory of video files of Television Series and rename them according to Plex's format.
Use theTVDB.com's API to find the best matches to current file names, and rename them accordingly.
https://support.plex.tv/articles/naming-and-organizing-your-tv-show-files/

# Milestones
It's easier to break the project into multiple Milestones. Milestones give the notion that big goals are accomplished. 
Each milestone should represent a fully functional piece of code. Each Milestone has multiple goals/requirements that should be met to form a functional program.
Goals in the Milestone should encompass a unifying theme. If a goal doesn't fit the milestone, it probably should be in another one.

# Milestone 1
## File Renaming
Prove that the code given a file directory, it can rename the files with a predetermined list of episodes.
### Goals
- Implement Plex file naming Convention
  - (tv_series_name) - s(season_number)e(episode_number) - (episode_title).(file_extension)
    - tv_series_name: name of the TV Series
    - season_number: Season number minimum of 2 digits 
      - 02 = is Season 2
    - episode_number: Episode number minimum of 2 digits 
      - 09 = Episode 9
      - 113 = Episode 113
    - episode_title: Title of the episode
- Read a list of episode titles and rename episodes
- Show a preview list of all changed and unchanged episodes
  - OLD_NAME.mkv --> (tv_series_name) - s(season_number)e(episode_number) - (episode_title).(file_extension)  # changed episode
  - OLD_NAME.MKV --> unchanged

# Milestone 2
## Acessing the TVDB API
Prove that the code, given an TV Show name, can save all seasons and episodes within the season.
### Goals
- Build tools to properly connect to the TVDB API
- Find TV Show and save episode names to a list of 
  
# Milestone 3
## Automation
The less manual input, the better. 
### Goals
- Find best guesses for name of TV Show based on current filename and directory path.
  - List all matches
  - Verify match with user
- Guess season number based on directory path and number of episodes
  - Check sibling directories for clues
  - If more than one match, list seasons.
- Match episodes based on the following:
    - File name/order 
    - Prexisting file attributes if given
      - Title
      - Episode runtime
- Handle split episodes
- Provide choice of destination path
  - Directory doesn't exist -> create it
  - Check to see if it is in a season folder
  
# Milestone 4
## GUI 1
The terrifying world of a Graphical User Interface. Plain Text edition!
### Goals
- Convert all terminal interactions into simple plain text interfaces

# Milestone 5
## GUI 2
Graphics are better than plain text
### Goals
- Show picture previews of TV show matches
  - TV Show Matches
  - Season Number Matches

# Miscellaneous Goals, Reqiurements, and Considerations
These are things that come to mind that are not in a Goal or Milestone yet.
