%%
#Complete
#Design
%%
# Validation of Inputs

## Metronome

| Function             | Input/s                   | Format           | Input Method                  | Range                                       | Justification                                                              |
| -------------------- | ------------------------- | ---------------- | ----------------------------- | ------------------------------------------- | -------------------------------------------------------------------------- |
| Input BPM            | BPM                       | Integer          | Inc/Decrement Buttons, Slider | 1<=x<=300                                   | Vast majority of music's BPM is within this range                          |
| Input Time signature | Top Number, Bottom Number | Integer, Integer | Sliders                       | 1<=x<=20, 1<=x<=16 where x is a power of 2. | Majority of music is within this range, Bottom number must be a power of 2 |
| Start/Stop           | isRunning                 | Boolean          | Toggleable button             | True,False                                  | There are only two valid states for any metronome, running or not running  |

## Practice Tracker

| Function             | Input/s | Format | Input Method | Range | Justification                                                                                                 |
| -------------------- | ------- | ------ | ------------ | ----- | ------------------------------------------------------------------------------------------------------------- |
| Record Practice Info | info    | string | Text field   | N/A   | User should be able to enter any characters they see fit, as long as it is understandable and useful to them. |
