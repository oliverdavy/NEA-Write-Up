%%
#Complete
#Design
%%
# Data Structures

Both halves of the solution will make use of appropriate data structures to ensure data is stored and retrieved in an effective and intuitive manner.

Within the metronome most data can be stored as simple variables.

| Name        | Type    | Description                                                               | Justification                                                                                                                                                            |
| ----------- | ------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| activeLight | Integer | holds the index of the currently active light                             | indexes are always integers                                                                                                                                              |
| currentBPM  | Integer | holds the current BPM of the metronome                                    | BPM is always an integer                                                                                                                                                 |
| active      | Boolean | false when the metronome is not running, true if the metronome is running | The metronome can only be in two state, running or not running, so a boolean which can only be two values is most appropriate                                            |
| beats       | Integer | holds the amount of beats per bar (the top number of the time signature)  | Whilst non-integers are used in time signatures, it is exceedingly rare and can always be converted to a time signature with integers, so an integer is most appropriate |
| subdivision | Integer | holds the subdivision of each beat (the bottom number of the metronome)   | Whilst non-integers are used in time signatures, it is exceedingly rare and can always be converted to a time signature with integers, so an integer is most appropriate |
For some data it is more appropriate for them to be stored within larger data structures

| Name       | Type         | Description                                                                                                                                  | Justification                                                                                                                                                                                                                                           |
| ---------- | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| trackSkips | boolean list | each index corresponds to a light. If the value of that index is false that light should be skipped. Otherwise it should be treated normally | As there are several lights that need to be tracked, the number of which can be changed at any time, a list was deemed best as it is dynamic. It was determined booleans were best as a light can only be in one of two states, skipped or not skipped. |

For the practice tracker it was expected data structures would generally be more complex, as operations involving databases are planned. 

A simple database diagram was made only involving one table

![sessions ER diagram](sessionsER.png)
>sessions table diagram

This table would simply hold all completed practice sessions, which would be given a unique id. They would also hold a date and info about the practice session itself. 

To access the database SQL would be used. The commands to facilitate this can be found in the algorithms section.

When loaded from the database into the program it was decided they would be best stored as a data class with fields for each of the fields in the sessions table.

![Sessions class diagram](SessionClass.png)
>session class diagram

