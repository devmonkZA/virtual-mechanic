


# Software Testing #

The project will use two frameworks to automatically test the software during development. They are:

  1. OCUnit: a unit testing framework for Objective-C that integrates with Xcode. The team writes test cases that include assertions about the code under test. Test suites are collections of test cases that are run uniformly by a test runner. When the tests are run, they check their own results and provide an unambiguous pass or fail message.

  1. X-Code Shark: A framework which also integrates with Xcode. It traces CPU and memory usage by processes and can reveal bottlenecks or areas that can be optimized by multithreading or rewriting of code.

## Test cases ##

**Main menu**

| **Input** | **Output** |
|:----------|:-----------|
| Click "Start" | Show list of machines to open |
| Click on a machine | Open the selected machine, and show the machine view with tabs below |
| Click on "Download new.." | Open the Download Machines menu |
| Click on "Download Machines" | Open the Download Machines menu |
| Click on a machine to download | Download machine and update the list of machines |
| Click on "?" | Show help menu |
| Click on "View topics" | Show all help topics |
| Click on "Search" | Show text field and keyboard for entering search term |
| Click "Report a bug.."  | Show text field and keyboard for bug reporting and submit button |
| Click "Settings" and manipulate options | Show settings menu and change settings as desired |


**Machine interaction**

| **Input** | **Output** |
|:----------|:-----------|
| Click on a component | Highlight component with red halo. Show name of component on title bar |
| Click on empty space | Un-highlight any component. Show "Overall" on title bar |
| Click on component and drag to left/right/up/down | Move component left/right/up/down |
| Release component | Anchor component to place where it was released |
| Click undo | Undoes previous action |
| Click "Details and Discuss" | Show comments page for component (if selected) or overall machine |
| Click "Post new comment.. | Show text field and keyboard for comments and a submit button |
| Click "Photos" | Show photos page for component (if selected) or overall machine |
| Tilt iPhone horizontally | Does nothing |
| Shake iPhone | Resets components positions (if setting is turned on!) |

Test cases will be added whenever there are new features or when a feature is found to have many bugs. During testing, the team will keep track of the number of failures and the severity of them. Features with high-importance should have no failures at all. All strange and unexpected behavior will be recorded, along with how they occurred. New test cases can then be created for them to avoid reoccurrences.


---


# Internal Deadlines #

| **Version** | **Action** | **Start Date** | **End Date** | **Supervisor** |
|:------------|:-----------|:---------------|:-------------|:---------------|
| 1           | Unit testing and Revision | October 30, 2009 | November 2, 2009 | Greg           |
| 1           | Integration testing and Revision | November 2, 2009 | November 4, 2009 | Tyler          |
| 1           | Submission | -              | November 5, 2009 |                |
| 2           | Unit testing and Revision | November 12, 2009 | November 14, 2009 | Chien          |
| 2           | Integration testing and Revision | November 14, 2009 | November 17, 2009 | Marc           |
| 2           | Submission | -              | November 19, 2009 |                |
| 3           | Unit testing and Revision | November 25, 2009 | November 28, 2009 | Jeff           |
| 3           | Integration testing and Revision | November 28, 2009 | December 1, 2009 | Greg           |
| 3           | Submission | -              | December 3, 2009 |                |


---


# User Acceptance Testing #
There shall be 2 user acceptance tests at different points of the implementation phase:

- The 1st test date is November 2, 2009 to gain a sense for anything that might be improved early on.<br>
- The 2nd testing date is November 17, 2009<br>
<br>
The testing will be done in two different locations, SFU and in an auto shop.<br>
<br>
<b>SFU</b><br>
There shall be tests conducted at SFU to test the software in an academic environment, with with university students of varying majors (focused around mechanics).  The tests shall be conducted in a variety of settings from load busy hallways to the quiet of the library. This is to test how quickly users can engage in the software in distracting or calm environments.<br>
<br>
<b>An auto shop</b><br>
The autoshop test shall test the viability of the software in a grungy environment, where the users might not have clean hands.  It will also be an opportunity to test the software with trades workers, some of whom have been to trade school, some not. Again the software shall be tested in load and quiet environments.<br>
<br>
<b>Testing Plan</b><br>
Case 1: The user will begin in the main menu and will be asked to open a machine by clicking the start button and selecting the machine, and then go back to the main menu by clicking the back button.  The user will then be asked to again click the start button and select a machine to load opening the machine view.  The user will then be asked to select a part and move it to a different part of the screen.  The user will then be asked to comment on the part, by clicking on the comment button.  The user will then click post and write a comment on the part and submit it to the server.  Finally the user will view the comments for that part and verify that it is on the device.<br>
<br>
A successful test: The test could be considered successfull if the user is able to navigate through all the windows as the description of the software says it should, the comment is actually posted, and if this test may be completed within 5 minutes.<br>
<br>
Case 2: The user will begin in the main menu, and will be asked to open the help window.  From here the user will be asked to search the help contents for a word of their choice.  The user will then be asked to go back and bring up the help table of contents and view a page of their choice.  Then the user will be asked to go back to the main menu and open another machine via the start button and selecting their machine.  The user will then be asked to select a part and view the photos for that part by clicking the photo button on the control bar.  When the user is viewing the photos the user will be asked to add a photo from their iPhone.  Finally the user will be asked to go to the photo viewing page and ensure that their new photo is there.<br>
<br>
A successful test: The test could be considered successful if the user is able to navigate through all the windows as the description of the software says it should, the photo is actually posted, and if this test may be completed within 5 minutes.<br>
<hr />

<h1>Integration Testing</h1>

The team shall incrementally integrate and test different components of the system during development. The basic menu features will be tested first, before moving on to viewing machines, interacting with them, and commenting on them, and so on.<br>
<br>
<b>Step 1 - Verify menu controls and help function</b>

Without opening a machine, a user should be able to navigate the menu properly, change any basic settings in the settings menu, and be able to view the help documentation at all times by clicking on the "?" icon.<br>
<br>
<b>Step 2 - Opening new machines</b>

Users should be able to open a machine, switch between machines, and selecting different components of the machine.<br>
<br>
<b>Step 3 - Dragging part of the machine</b>

Components should be moveable by selecting them and moving them with the user's fingers. The following bugs may occur:<br>
<br>
<ol><li>If we want to drag any part of the machine, a possible bug may be that users cannot select the part that users would like to drag. This may be because components are too close together, or that the particular component is not selectable.</li></ol>

<ol><li>While dragging a part of the machine, delay may occur due to slow processing speed or other non-functional reasons. For example, the images cannot follow the moving of our finger. In the worst case, it may take 5-10 seconds before seeing the moving of components</li></ol>

<ol><li>If we are dragging a part of a machine, and the coordinates are calculated wrongly, then the images would not move to exactly where the users want them to be.</li></ol>

<ol><li>While moving a component from one place to another and it passes by another component, the program must not allow users to also drag the images were passed by.</li></ol>

<b>Step 4 - Posting new comments and photos</b>

In this high-level test, the user would try to view and post comments or photos to the server. The following issues may occur:<br>
<br>
<ol><li>If the users type the font that iPhone cannot display the code of the font then it would be shown as confused symbols that cannot be read. Thus, restrictions need to be made on the allowed font, language, colours and size.<br>
</li><li>If the users cannot connect to the server, then their comments and photos are not uploaded.<br>
</li><li>Network errors may occur, causing data that are not received properly. However, this is not an application layer problem but a network or data link layer problem which is out of the team's scope.<br>
</li><li>Images which are too large to upload are rejected. (Max size is 300kb)<br>
</li><li>Discriminatory or vulgar comments need to be filtered.</li></ol>

<b>Step 5 - Downloading new machines</b>

Users should be able to download new machines within 10 minutes and view them immediately with no additional settings. They must also be able to perform all the functions listed above.<br>
<br>
<hr />

<h1>Size and complexity</h1>

<table><thead><th> <b>Version</b> </th><th> <b>Lines of code</b> </th><th> <b>Number of classes</b> </th><th> <b>Number of files</b> </th><th> <b>Number of machines</b> </th><th> <b>Program size</b> </th></thead><tbody>
<tr><td> 1              </td><td> 200                  </td><td> 5                        </td><td> 5                      </td><td> 1                         </td><td> 1MB                 </td></tr>
<tr><td> 2              </td><td> 500                  </td><td> 6                        </td><td> 10                     </td><td> 2                         </td><td> 2MB                 </td></tr>
<tr><td> 3              </td><td> 800                  </td><td> 7                        </td><td> 15                     </td><td> 2/3                       </td><td> 3MB                 </td></tr></tbody></table>

Software tools will not be mandatory for keeping track of the project complexity. Instead, the team will record the actual numbers from observations (ie. noting the number of lines in the xcode, recording the total size of the project folder, etc.) and continuously update these figures.<br>
<br>
If the project grows too large to keep note of numbers by hand, then "Xcode Menu Script" can be used to automatically count the number of lines of code. "Code Sense" is another Xcode tool which can be used to view all the classes during development.<br>
<br>
<hr />

<h1>Miscellaneous Quality Assurance</h1>

<ol><li>Document progress in a thorough manner.<br>
</li><li>Have supervisors for each testing phase for added assurance.<br>
</li><li>Take notes through each use case testing to document errors.<br>
</li><li>Continuously update requirements documents.<br>
</li><li>Notify users of program updates/documentation.<br>
</li><li>Appoint a team member as Assurance Officer.<br>
</li><li>Weekly group meeting to discuss progress.</li></ol>

<hr />