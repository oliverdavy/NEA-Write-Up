%%
#Complete
#Design
%%
# Identify Test Data

## Milestones

- [x] Create the metronome interface
- [x] Start and Stop the Metronome
- [x] Change the BPM
- [x] Change time signature
- [x] Add skip beats
- [x] Change between metronome and practice tracker screen
- [x] Display list of past practice sessions
- [x] Start new practice session
- [x] Save, load, and delete sessions


## Tests

### Milestone 2: Start and Stop the Metronome

| Test Number | What is being tested and inputs                                                                                        | Expected output                                                                                                                           |
| ----------- | ---------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| 1           | The start stop button changes the state of the metronome from running to not running and vice versa. Test: true, false | When the running state is 'false' it will change to 'true' upon use. When the running state is 'true' it will change to 'false' upon use. |
| 2           | The start stop button changes appearance based on if the metronome is currently running. Test: true, false             | When the running state is 'false' it will display a play icon. When the running state is 'true' it will display a pause icon.             |
| 3           | The light stored as the currently active light is displayed as lit. Test: -1, 0, 3, 4, H                               | A number from 0-3 is accepted (default amount of lights is 4). All other inputs rejected                                                  |
| 4           | The currently active light is correctly incremented.                                                                   | The next light is lit as the current becomes unlit. This rolls around to the start if the final light is reached.                         |
| 5           | The lights are updated at a constant interval based on the current BPM. Test: 0, 60, 300, 301, 350, H                  | Lights update at a rate inversely proportional to the current BPM. Numbers from 1-300 are used, any others rejected.                      |
### Milestone 3: Changing BPM

| Test Number | What is being tested and inputs                                                       | Expected output                                                                                                                                                                                 |
| ----------- | ------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1           | BPM can be incremented and decremented from various values. Test: -1, 0, 60, 300, 301 | BPM is incremented and decremented from valid values (1-300). It does not increment or decrement to invalid inputs. If the initial value is invalid it is corrected to the closest valid value. |
| 2           | BPM can be updated using a slider.                                                    | BPM updates to match the position of the slider. This also works in reverse, with the slider position updating to the BPM if it updates via other means.                                        |
### Milestone 4: Changing Time Signature

| Test Number | What is being tested and inputs                                                | Expected output                                                                                               |
| ----------- | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------- |
| 1           | Number of lights updates to match the current number of beats (the top number) | Number of lights equals top number within valid values                                                        |
| 2           | Speed of beats updates to match current subdivision.                           | speed of beats is  proportional to the subdivision i.e. a doubling in subdivision causes a doubling in speed. |
### Milestone 5: Adding skip beats

| Test Number | What is being tested and inputs | Expected output                                                                                 |
| ----------- | ------------------------------- | ----------------------------------------------------------------------------------------------- |
| 1           | Beats can be toggled on and off | Beats which are toggled off are always treated as inactive. Otherwise they are treated normally |
### Milestone 6: Starting a new practice session

| Test Number | What is being tested and inputs                                               | Expected output                                                                                         |
| ----------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| 1           | A new practice session can be started                                         | An interface is generated with all necessary components of the practice tracker                         |
| 2           | A timer is used to track the length of the practice session and can be paused | A time starts and counts correctly at the correct speed. It pauses and plays when requested by the user |
| 3           | The date and time is recorded automatically                                   | The date and time of the session are retrieved and displayed correct with the current time and date.    |
## Milestone 7: Saving, loading, and deleting a session

| Test Number | What is being tested and inputs                                 | Expected output                                                                |
| ----------- | --------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| 1           | Practice sessions are stored into a database correctly          | The database is shown to be storing the sessions with all data intact          |
| 2           | Practice sessions can be recalled from the database into memory | The database is queried and returns the desired session with all relevant data |
| 3           | Practice sessions can be deleted                                | The desired session is deleted from the database                               |



