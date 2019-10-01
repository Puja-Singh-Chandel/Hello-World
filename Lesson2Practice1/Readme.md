# Working with Notepad Application

In this practice session, I have explored working with Windws Notepad application. 
The project asks user to choose whether the expression shown is correct or not, it then types the users selection result in the Notepad Window.
Both FlowChart and Sequence have been put to use here. The activities used are :MessageBox, Flow Decision, Assign, Open Application, Attach Window, Type Into, do , Click and Close window, Close Application.

Note:
If you use Close Application activity, the Save dialog box cannot be handled by Click activity on 'Don't Save' button. This can be taken care of if "Close Window" activity is used. This could be because of force closure in case of " Close Application" activity.
as per discussions in UiPath forum.

## Getting Started
Download the file or clone in to your local machine and open it through the UiPath Community edition.
No additional packages required.

## Problem Statement
Start by asking the user a mathematical question (e.g. the equation, 1+1 =2) in a Message Box with Yes/No choices and capturing the user's answer:

* If the user answered Yes (which is the True answer): 
  + Opens Notepad.exe
  + Attaches to the window of Notepad.exe
  + Upon attaching to the window, types Correct into it.
* If the user chose No (which is the False answer):
Does the same series of actions as the True branch. However, instead of typing Correct, types Incorrect into Notepad.

Finally, closes the Notepad application.

## Acknowledgments
[UiPath Forum](https://forum.uipath.com/t/whats-the-difference-between-close-application-and-close-window-why-does-uipath-behave-different-after-one-or-the-other/85962)


