%%
#Development 
%%
The goal of this iteration was to setup android studio with a default project and to make it so GitHub could be used for version control. The default project was not edited in anyway during this iteration. It was built and deployed on my device via ADB (Android Device Bridge) and a google pixel 3a emulator to test it worked so that development could be done efficiently in future iterations. All testing is documented in the completed test plan below 

 After the default project was made it was committed as the initial commit to the GitHub page to test it was working so that version control could be managed easily, allowing for
 easier tracking of progress as features are implemented in future iterations.

![Iteration One](/iteration1.png)

| Test  <br><br>Number | Test Description                                                                                                                        | Test Data                                    | Test Type | Expected Result                                         | Result  |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- | --------- | ------------------------------------------------------- | ------- |
| 1                    | Testing android studios android studio Google Pixel 3a emulator functions                                                               | The default generated Android studio program | Valid     | The program builds and deploys to the emulated pixel 3a | Success |
| 3                    | Testing android studios ADB functions with my hardware (Oppo phone thingy) [make sure to change this and figure out what your phone is] | The default generated Android studio program | Valid     | The program builds and deploys to my device correctly   | Success |
| 2                    | Testing the ability to make commits of the current program state to GitHub                                                              | The default generated Android studio program | Valid     | Data is accepted and successfully uploaded              | Success |
