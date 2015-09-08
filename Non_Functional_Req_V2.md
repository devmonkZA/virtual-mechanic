# Non-functional Requirements #
## Product Requirements ##
Product Name: virtual-mechanic
Created by: Virtual Mechanics (Group 12)
Proposal: Allow users to analyze a machine by virtually disassembling the machine and inspecting the individual components that it is comprised of.
Users: This application will be built such that any iPhone user may use it without difficulty.
Reliability: The application is designed to run smoothly on the iPhone platform. For internet access (i.e. downloading content) there should be no delay other than the regular downloading rate the user regularly experiences with their iPhone.

### Usability Requirements ###
After 10 minutes of experience with the software, an iPhone user with at least 5 hours of iPhone experience should be able to perform any of the functions when asked, with no training necessary.

### Performance Requirements ###
The Following functions should be performed with no noticeable delay:
  * Selecting a part
  * Dragging a part
  * Zooming in the Machine view or when viewing a photo


The following functions should be performed within 1 second:
  * Switching between any of the windows

### Space Requirements ###
The program itself will take up at most 10MB of flash drive space.

Each machine will require space for:
  * MachineView.txt (About 29bytes + 230Bytes/component)
  * Description.txt (max 500 characters(500bytes))

Each machine component will require space for:
  * MachineViewImage.png (max 40KB)
  * Description.txt (max 500 characters(500bytes))

### Reliability Requirements ###
If the user performs an illegal operation, error checking methods will be initiated and the program will either ignore the operation or alert the user, depending on the situation.


## Organizational Requirements ##
### Standards Requirements ###
Current coding standards accepted for the iPhone and Objective-C will be followed for this project.


Names of All UIViewController subclasses must follow the format:  class's service + ViewController
ex:  PhotoViewController  means a UIViewController subclass that displays photo of components of machine.

all class header should include:<br>
<blockquote>Person Worked on: <br>
Change History: <br>
Problem to be solved: <br>
Description: <br></blockquote>


Important and methods  that is not easy to be understood should begin with<br>
@description:<br>
@parameters:<br>
@precondition<br>
@postcondition<br>

All variable names should be self-explainatory.</br>


<h3>Delivery Requirements</h3>
This application requires the application’s executable file to run, as well as all related source code. Also, all of the data such as component images and related comments will be delivered from the server, and can be accessed from the download a machine feature.<br>
<br>
<h3>Implementation Requirements</h3>
The software will be developed using the XCode programming environment, SDK 3.0, in the Objective-C programming language. The GUI will be fine-tuned using the XCode Interface Builder. The software will run on Mac OSX on the iPhone platform. The frameworks involved are: Cocoa touch, CFNetwork. The online user interactivity will be based on an FTP server.<br>
<br>
<br>
<h2>External Requirements</h2>
Comments and photos for each part will be stored in an FTP server as associations of each machine that has been uploaded.<br>
<br>
<h3>Interoperability Requirements</h3>
The requirement of importing this application to a machine (computer, cellular-phone, etc) is the operating system. The operating system must be Mac OSX with iPhone SDK 3.0 or greater.<br>
<br>
<h3>Ethical Requirements</h3>
This software is intended for educational purposes and is meant to be distributed freely. Any costs incurred will be those associated with the user’s current data plan on their iPhone account upon downloading the application. This is a public application and so every uploaded ‘machine’ will be screened for offensive content before being released for download.<br>
<br>
<h3>Privacy Requirements</h3>
The Virtual Mechanic application will never ask for the user to submit any personal information aside from a user name. Moreover, the application will not upload any users' information to the server or any third-party.