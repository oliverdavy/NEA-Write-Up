
%%
#Complete
%%
# Research

#### Existing Systems

##### Metronome Online

![Metronome Online](Metronome%20Online.png)
>Metronome Online

Metronome online is accessed via a web browser as a website ([https://www.metronomeonline.com/](https://www.metronomeonline.com/) Accessed at 2024/06/27). The metronome is presented as a circle where different BPMs are selected by clicking on labelled buttons around the circle. The start/stop button is prominent in the centre and shows the currently selected BPM. It also includes the Italian names for tempo. The two large arrows at the side allow for fine tuning of the tempo in increments of one BPM. Underneath the main UI is a timer for how long the metronome has run, a tap button to allow the desired metronome to be tapped in by the user, and a second timer for how long the metronome has run in total that day. Above is a small volume slider. To the left is a menu. Upon expansion (see below) the menu shows a variety of customisation options. These allow for variation in time signature, Sound style, Dark/Light mode, and to play an A at 440hz for tuning.

![Metronome Online Customisation Menu](MetrOnlineMenu.png)
>Metronome Online Customisation Menu

The expanded menu allows for greater customisation, which is not an immediate necessity, unlike the other options shown in the main menu. The time signature has two drop downs to select the number of beats and the division of said beats. There is also a further settings menu next to this. The sound style also has a drop down to select the various sound options. The dark mode and tuner are toggled by simple switches.

![Metronome Online Time Sig. Customisation Menu](MetrOnlineTimeMenu.png)
>Metronome Online Time Sig. Customisation Menu

The time signature settings show the same drop downs as one the previous menu. It also allows adjustment to the accent on each beat from four levels (zero to three). It shows the tempo below. It also allows for different subdivisions of time to be played each beat. It allows for no subdivision, duplets, triplets, and quintuplets. There is also a reset button

##### Google Metronome
 
![Google Metronome](GoogleMetr.png)
>Google Metronome

 The google metronome is accessed directly from the browser by searching for metronome. It very simply has a text box to display the current BPM, a start/stop button, and a slider to select the BPM. The drop down below links to other tools like this made by Google and is not relevant to the tool itself. The colour of the UI changes with higher and lower BPMs varying from colder colours to warmer colours.

![Google Metronome Cold](GoogleMetrCold.png)
>Google Metronome Cold

![Google Metroome Warm](GoogleMetrHot.png)
>Google Metronome Warm

##### Metronome Beats

![Metronome Beats](metronomeBeats.png)
>Metronome Beats

Metronome Beats is an android app developed for use on mobile devices. It features two modes, a metronome and a drum machine. For this project, the metronome will be the focus of analysis.

The side menu features links to other apps by the same developer as well as premium features which have no impact on the metronomes use, so it will be ignored. The mode select allows for switching between the two different modes. While it may appear there are five modes, the middle button is a simplified drum machine, the generates poly-rhythms on the drum machine and does not open a separate page, and the last button prompts the user to purchase premium features; so for practical usage, there are only two modes.

The lights indicate which beat the metronome is currently on by turning on and off. The first beat is coloured differently for emphasis.

The sliding indicator moves linearly back and forth, returning to the start every other beat.

The increment and decrement buttons can adjust the BPM by one and five. The BPM display can also be used to adjust the BPM by scrolling it. The BPM slider can also be used to adjust the BPM. It also features a written tempo written above it, which changes based on the range the current BPM is within.

The beats/bar button opens a popup menu to change the amount of beats in each bar from one to sixteen. The clicks/beats button opens a popup menu to change the amount of click sounded per beats from one to sixteen. The tap tempo button adjusts the tempo to how often it is being pressed by the user.

The start/stop button is used to start and stop the metronome. The tempo trainer opens a separate screen to add a count in, increase and decrease tempo after a certain amount of time has passed, and add mute bars. the timer button opens a separate screen to add a count in, and stop the metronome after either a certain amount of bars, or a certain amount of time. It also allows the amount of time elapsed to be shown, but is off by default.

##### Musicalog

![Musicalog](Musicalog.png)
>Musicalog

The home page features two sections, one to show current goals (of which there are none by default), and one to show the progress of total time spent practising. There is a button to buy premium which will be ignored, as well as a button to start a new practice session. There is also a section at the bottom to switch between four pages, home, log, view, and options.

The log page shows a large button to start a practice session along with a smaller button to add previous practice sessions.

![musicalog default log page](musicalogLog.jpg) 
>Musicalog log page

When practice is started a stopwatch begins counting. At the bottom there is a pause button along with a button to end practice. There is also a button to create an archive. Archives are used to record audio.

![musicalog timer](musicalog%20timer.jpg)
>Musicalog Timer

Once the finish button is pressed a screen to save details about the practice log is opened. There are text fields to record instrument, date, time spent, as well as any notes. The instrument field can auto-fill common instrument names as well as changing the eighth note icon to match.

![musicalog save](musicalog%20save.jpg)
>Musicalog Save Session

On the view page previous practice sessions can be viewed and filtered by date and instrument. The total practice time progress tab is reused from the home page.

There are several possible behaviours for the timer during sessions, which are selectable from the options page. By default it will check if any practice goals are active. If none are found it will use progress within an hour. Progress within hour will cycle between zero percent to one hundred percent every hour e.g. at three hours forty five mins it will show seventy five because it is currently three quarters through the current hour. If at least one goal is set, then it will switch to goal progress.  Goal progress shows progress towards a set goal. e.g. if goal was twenty hours in a month and you had done ten so far it will show fifty percent. Progress within hour and Goal progress can both be set to be the default option. The final setting is Progress to fixed time which will show how close a session is to reaching a specified time. e.g. if time set was one hour and it had been fifteen minutes it would show twenty five percent. 

Logs can be imported and exported as CSV files as well as be completely wiped. Archives can also be exported or imported via CSV. 

##### Common Metronome Features

- set bpm

- start stop button

- tap bpm

- time signature

- customise sounds

- subdivisions

- customise appearance

- skip beats

##### Common features practice logs 

- timers

- goals

- review sessions

- record bits from sessions 

- stats

#### Stakeholder Needs

A google form was sent to stakeholders. It asked what they believe is essential in a metronome/practice tracker, and what is nice to have. 

The essentials for a metronome were: keeping track of rhythm 

- making sound 
- changing and showing speed
- range of selectable time signatures
- visual reference e.g. lights

Nice to have features of a metronome included:  

- being able to save presets
- changing the noise made
- beats per second instead of per minute  
- Vibration
- emphasis on certain beats
- ability to play over a song  
- list of popular music with their tempos and time signatures  

Essential features of practice log: 

- Date and duration of practice
- Record of what was practiced
- Notes e.g. good and bad parts, what to improve
- Ability to start and stop timer

Nice to have features of practice log: 

- Share option
- Statistics on practice
- Automatically start logging when app is opened
- Streaks (like duolingo)
- Session tags (e.g. scales, classical, etc.) perhaps linked to metronome presets 
- Attach sheet music 
- Instrument played

#### My Ideas and Approach

I agree with the ideas that were suggested by the shareholders. I also think audio recordings should be added, as I think it would be useful for reflecting on tone and intonation. Furthermore, I believe video recording could be added, but would be of less priority. I think this would be helpful in analysing technique