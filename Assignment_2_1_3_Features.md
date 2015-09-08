

First Some terms (these shall be moved to the Glossary later)

Machine: A composition of images of different parts of a machine, placed on top of each other to recreate the machine as viewed from some angle.  As well as a collection of comments associated with the parts and with the machine itself.

Machine View: Is the view of the Machine where one may disassemble it, and select different parts.


# Features #

  * [View Machines](http://code.google.com/p/virtual-mechanic/wiki/Assignment_2_1_3_Features#View_machines)
  * [Download new machines](http://code.google.com/p/virtual-mechanic/wiki/Assignment_2_1_3_Features#Download_new_machines)
  * [machines) Drag and drop (disassemble machines)](http://code.google.com/p/virtual-mechanic/wiki/Assignment_2_1_3_Features#View_machines#Drag_and_drop_(disassemble)
  * [Commenting](http://code.google.com/p/virtual-mechanic/wiki/Assignment_2_1_3_Features#Commenting)
  * [Photo posting](http://code.google.com/p/virtual-mechanic/wiki/Assignment_2_1_3_Features#Photo_posting)
  * [Layered images](http://code.google.com/p/virtual-mechanic/wiki/Assignment_2_1_3_Features#Layered_images)
  * [Help/Instructions](http://code.google.com/p/virtual-mechanic/wiki/Assignment_2_1_3_Features#Help/Instructions)

## View machines ##
## Drag and drop (disassemble machines) ##
## Download new machines ##
## Commenting ##
## Photo posting ##
## Layered images ##
## Help/Instructions ##




# Features #

---

## Main Menu ##
The main menu shall show the logo, and name of the product, as well as 5 buttons at the bottom of the screen, which offer the following options:

### Load Machine ###
Allows the user to load a **machine** which is saved onto the device (excluding comments on **parts** and the machine itself)

### Download new Machines ###
Allows the user to download new machines from the server

A button in the main menu opens up a catalog of machines available for download.

### Settings ###
Help: on/off<br>
Shake-to-reset: on/off<br>
OR<br>
Shake-to-randomize: on/off (mixes up the part positions)<br>
Background colour: automatic/set color  <----(Can we get a color wheel for this or can we only offer finitely many colors?)<br>
Sound: there will be sound while user doing action such as dragging a <b>component</b> to somewhere or shake to reset. <br>
Automatically download new content?<a href='http://code.google.com/p/virtual-mechanic/w/edit/Assignment_2_1_3_Features'>http://code.google.com/p/virtual-mechanic/w/edit/Assignment_2_1_3_Features</a> <br>
Send anonymous usage report to server?<br>
<br>
<h3>Program feedback</h3>
A button in the main menu links to a form that allows users to give feedback on the application.<br>
<br>
<h4>Help</h4>
The Help button brings up the help table of contents.<br>
<hr />
<h2>Viewing the Machine</h2>
<h3>The Control Bar</h3>
The control bar is present whenever the user is viewing a machine.  It is displayed at the bottom of the screen and contains 5 buttons:<br>
<h4>Reset Button</h4>
The reset button returns all the parts of the machine to their default location<br>
<br>
<h4>Commenting Button</h4>
The commenting button allows users bring up the comment window for the currently selected part.<br>
<br>
If no part is selected it brings up the comment window for the machine.<br>
<br>
If the comment window is already open it closes the comment window (returning the machine view)<br>
<br>
<h4>Photo Button</h4>
The <b>Photo</b> button brings up the photo window for the currently selected part.  If no part is selected then it brings up a photo window for the machine.<br>
<br>
<h4>Help Button</h4>
The help button brings up a help window which gives the user advice about the screen they are currently looking at.  Its precise behavior for each window is described below in the description of each window.  From each help window one can navigate to the help table of contents via a link at the bottom of the page, or go back to your previous window by again clicking the help button.<br>
<h4>Main Menu</h4>
Returns the user to the main menu<br>
<hr />
<h3>The Machine view</h3>
The Machine view is the screen where the user may view and interact with the machine.<br>
<h4>Disassembly</h4>
By using their fingers, users can take a machine, apart piece by piece. Using a "click-and-drag" interface, users can place the pieces anywhere they wish on the screen. Since the machine is built with many overlapping images, users can view the deeper components by dragging the upper images to other places on the screen.  <br>
In addition to viewing the deeper image, users can drag to zoom to a specific component they want to look at in detail.<br>
<br>
To select a part: The user taps the <b>layer</b> with their finger.  The name of the part is displayed at the top of the screen to show that the correct part has been selected.<br>
<br>
To deselect a part:  The user may tap empty space.<br>
<br>
To move a part:  Once the part is selected the user may press and hold their finger over the layer and then drag the layer to the desired location.<br>
<br>
<h4>Zooming</h4>
Using two fingers to tap and expand on the screen will zoom in to the machine. To be more precisely, the screen will start zooming in from the place where the two fingers tapped at beginning. So the users can decide where to zoom in. When looking at photos, the action zooms into/out of photos.<br>
<h4>Help Button (On the Control Bar)</h4>
The help button on this screen brings up a help window which describes the Machine View and all functions available to the user here.<br>
<hr />
<h3>The Comments page</h3>
The comments page replaces the view of the machine leaving visible the control bar and the name of the part at the top of the screen.  The comments page will display 10 comments per page, with the option to skip pages at the foot of each page.  Each Comment will contain the following information:  Posters name, heading, date posted, and the comment itself.  The first comment will be stored inside the Ipod and will be a basic description given by the Machines creator.  The rest shall be loaded from the server and displayed in the format described above, or if no connection to the server may be achieved a single post shall be added which contains only the comment: Could not connect to server.<br>
<h4>Close Comments (On the Control Bar)</h4>
The user will be able to close the comments page by again clicking the Comments button.<br>
<h4>Post Reply Button</h4>
The option to post a rely will be given after the last post on that part, by the post reply button centered below the last post.<br>
<h4>Help Button (On the Control Bar)</h4>
The help button on this screen brings up a help window which describes the comments page and all functions available to the user here.<br>
<hr />
<h3>The Photo page</h3>
The photo page replaces the view of the machine leaving visible the control bar and the name of the part at the top of the screen.  The photo page will display a list of entries separated by horizontal rules each containing: A picture, a user name, date posted, and a comment.  All of the photo entries shall be loaded from the server and if no connection to the server may be achieved then a single entry shall be displayed on the page containing a comment stating: Could not connect to server<br>
<h4>Close Photos (On the Control Bar)</h4>
The user will be able to close the comments page by again clicking the Photo button.<br>
<h4>Post Reply Button</h4>
The option to post a rely will be given after the last post on that part, the post reply button centered after the last post.<br>
<h4>Help Button (On the Control Bar)</h4>
The help button on this screen brings up a help window which describes the Photo page, and all functions available to the user here.<br>
<hr />
<h2>Search</h2>
A button in the main menu links to a search page. Here, users can type the key word in search engine to search for a part which will show on the screen in Iphone and find part descriptions, comments from others, photos, etc.