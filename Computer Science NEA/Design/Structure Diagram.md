%%
#Complete
#Design
%%
# Structure Diagram

Since this project is made of two main parts, it seemed fitting to create a structure diagram for both.

![Metronome Structure Diagram](MetronomeStructure.png)
>Metronome Structure Diagram

Within the presets section, the state of the metronome can be saved and reloaded at a later time. Save Preset would create a record of all current variable values. Load Preset would overwrite all current variables with the values stored in a stored record.

The Start/Stop section handles the main running of the metronome. Each of its components will trigger periodically based on the current BPM, time signature, and skip beats and if the metronome is running. Start/Stop itself is responsible for keeping track if the metronome is running, changing this when appropriate. Update Lights increments which light is active each beat. Play SFX plays a sound effect on each beat. Trigger Haptics vibrates the device on each beat.

The BPM section is responsible for all BPM inputs.

The Time Signature section is responsible for controlling how many beats are played, at what subdivision, and keeping track of what's skipped. Input Time Signature handles the first two of these, as they are both encapsulated by the musical concept of a time signature. This is made of two numbers, a top number which encodes the number of beats per bar, and a bottom number which encodes the subdivision of each beat in a bar. For example 6/8 would mean that each bar of music has six eighth notes. Skip/Emphasise Beats tracks which beats should be played and skipped and provides a method for changing which beats are skipped.

![Practice Tracker Structure Diagram](TrackerStructure.png)
 >Practice Tracker Structure Diagram

Within Start Session there are three sub-sections, which will be used when creating a new practice session. Within Practice Info any information about the session is recorded. Date and Duration will keep record the date the session was made as well as the current value of the timer. Record Practice Info will record any user created notes on the session. End and Save will take all records from the other sub-sections and store them into a data base. The session is then ended and is able to be viewed in the Review Sessions section.

Review Sessions allows for past sessions to be viewed and manipulated. View Session allows all details of a past session to be seen. Share Session allows a session to be exported as a file. Edit Session allows details of a session to be edited after it is finished. Delete Session allows for a session to be removed from the database.

