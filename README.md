# AE125_Application

AE 125 Application  
Documentation 
 
The following documentation provided explains the entire ins and out how to use the application. Each step will include guidance on how to navigate the various elements found throughout the application.  
 
Disclaimer 
 
The application requires users to allow access to both Location information as well as Camera usage. It also requires access to the users’ file system.  
1.	Location information is required such that the application can automatically handle where the user is in the world. It gathers information about longitude, latitude, compass north, day of year, leap year and time to help calculate the user’s relative position on the Earth, therefore calculating where the sun is located with respect to the user. Without access, the application cannot function, as it would not be able to retrieve crucial information.  
2.	Camera is required as this is an Augmented Reality (AR) application. Camera access allows the user to place models into their phone screen while also seeing the real world simultaneously. Without access, this application would be Virtual Reality (VR) which is not the intended outcome. 
3.	File system is also required, as that is where the application will be pulling the users’ model from. The application only ever has access to the file currently imported (1. Select Model). The application will never read other file data that is not imported, and the application will never save into the users’ file system. Without it, users would have to find alternate methods to upload their models into the application.  
 
Introduction 
 
This application allows its users to place predominantly architectural models into scene space. For a long time, the field of architecture lags other industries in the realm of AR. This application is a stepping stone to help understand more whether AR is a viable and valuable resource in the architecture (as well as engineering and construction) industries.  
 
This documentation will demonstrate step by step how to use the application, as well as the various User Interface (UI) experiences throughout the application. It will be mainly split into two sections: Model Selection Screen and AR View Screen.  
 
Model Format 
 
This application accepts .gLB file type (Graphic Library Transmission Format Binary File). This format allows the model to carry material definition which provides another layer for realistic models. Modeling software such as Rhinoceros 8 and other model software allow exports directly to .gLB file type. Once the model has been exported, save the model to the native file folder in a location that is easy to access.  	 
Model Selection Screen 
 
The below image highlights the Model Selection Screen. Each area is indicated by a value and will be discussed in the proceeding sub sections.  
 
 
1.	Select Model 
 
Begin by pressing on the button called “Select Model (.GLB)”. Here Apple’s native file system will open to the Recent page. Navigate through and find where the location of the model. The only acceptable model format is Graphics Library Transmission Format Binary file (.gLB). However, Graphic Library Transmission Format (.gLTF) is also accepted, though due to the increase in file size, it is recommended to use the .gLB file instead. Once navigated, select the file which is to be displayed in AR. 
Below is text that reads “No file selected”. So long as no file has been selected, this text will remain as is. Once a file is selected, this will repopulate with the name of the file. So long as the file’s name is correct, this section is complete. Of course, models can be repeatedly change by simply pressing on the “Select Model (.GLB)” button.  
 
2.	Go to AR View (Next Scene) 
 
By pressing this button, the scene will change to the next (AR View Screen). By pressing this button, the current scene 
(Model Selection) cannot be accessed until a button is pressed in the AR View Screen (Page 3) 
 
3.	North Direction Override 
 
At the top is text defaulted to “North Direction: XXX.XX”. In this case, the direction is 163.95. This value will automatically read the initial northern compass direction upon beginning the application. The north direction is the value of the internal compass facing the direction of the camera. This information will be passed through to the following scene for mathematical calculations.  
Though on most occasions, the imbedded Apple compass may be inaccurate. To test for such, it is recommended to have either a true magnetic compass, or another phone/device that can be used to average out the compass direction. 
If wildly inaccurate (off by more than 5 degrees), please turn on the toggle switch.  
By toggling ON the “Override North”, the text “North Direction: XXX.XX” will read 0.00 unless a value had already previously been inserted into the text box “Enter North Direction” below. When the toggle is turned ON, it will overwrite the North Direction of the game with the user inputted compass direction.  
Upon entering the following scene and coming back to the home screen, the Toggle will remain in its position as well as either then internal compasses North Direction or the users North Direction.  
When the toggle is then turned OFF, the original North Direction read by the phone at the start of launching the game will revert to its original state.   
For accurate images, it is recommended to try and match the game compass North Direction as closely as possible to the true North Direction the phone is facing. Without such, the application may not look realistic at all.  
 
AR View Screen 
 
The below image highlights the Model Selection Screen. Each area is indicated by a value and will be discussed in the proceeding sub sections.  
 
 
 
1.	Toggle UI 
 
Three toggles are present in this scene. Each toggle is ON when there is a check mark contained in the box and OFF when the box is empty. Each toggle provides a valuable function to the application.   
 
a.	Occlusion Toggle 
 
Occlusion is still currently in its Beta Phase. It is complete in the sense where it will occlude, however it is not 
complete in the sense where there are still clashes, epically between the ground and the detected plane. It is still usable, though the quality is not on par to the rest of the model and remaining  
In this beta, occlusion begins OFF. This means that objects placed into the scene do not react to real world items. Upon turning ON, occlusion is now in progress, occluding both the environment as well as human occupants. Environment allows real world objects to block out the virtual model if placed behind. Human occlusion does the same thing, though rather than environment, it’s actual human. This means that when others go an interact with the model, the model behind them is not visible.  
 
b.	Lock Object Toggle 
 
Lock Object allows the users to continue touching the screen without worrying about moving the object. Initially when this Scene loads, the first time the user touches the plane, the set model will load. If the model isn’t located in the correct position, users can continue to touch the plane until the location of the model is accurate. After, the toggle can be turned ON. This allows the user to continue touching around the plane without having to worry about moving the model. This essentially acts as an anchor, locking the model to the real world. If at any time the user wants to relocate the model, simply switch the toggle to OFF and the object can be moved again.  
 
c.	Lock Screen Rotation 
 
Lock Screen Rotation toggle allows the user to choose whether to force the screen to face in one orientation or allow it to freely rotate. The application is built such that the user can either view their model in right-side up portrait mode, or either left or right landscape mode. If at any time the user wants to prevent the screen from rotating, simply turn the toggle ON. This locks the screen orientation, preventing unwanted rotation. If at any point the user wants to reorient the screen, turn the toggle OFF and it is free to change.  
 
2.	Hide UI 
 
Hide UI is a quintessential button that allows the user to remove all UI elements from the screen. To produce high quality images from this application, turning off all UI elements provides a clean screen with just the environment and the model placed in it. When the button is pressed, even itself will be hidden. To bring back the UI elements, press the same area the Hidden UI button was located. The Hidden UI button is mapped to roughly 300 by 300 pixels at the bottom left-hand corner of the screen. It will always be at the bottom left corner, no matter how the screen is oriented.  
 
3.	Back to Model Selection 
 
Back to Model Selection is a button that allows the user to return to the initial start-up Model Selection scene. Upon pressing, no data is stored, everything is wiped, and a clean slate scene will be available upon returning to the AR View scene. This includes the model that was placed alongside any toggles turned on or off.  
 
 	 
 Step by Step guide to using the Application 
 
The following section will be a quick step by step of a typical use case of the application.  
 
1.	Upon opening the app, click the Select Model button.  
2.	Select the model that will be used in the following scene. Make sure the model is a .gLB file.  
3.	After the file is chosen, double North. If within an acceptable range (plus or minus 5 degrees), continue by pressing the view in AR button 
a.	If the difference in angle is large, please select the toggle to overwrite the North Direction. Insert the North Direction in the input field and press enter. Once the North Text displays the correct north, proceed by pressing the view AR button.  
4.	The view AR button should be pressed, and the new scene should appear.  
5.	Allow the application a couple of seconds to initialize and start the plane detection.  
6.	Tap anywhere on the ground to begin placing the model.  
7.	If the location of the model is not to satisfaction, continue to tap around the plane until a suitable location is found.  
8.	Turn ON the Lock Model toggle.  
9.	Press the Hide UI to begin looking at strictly the scene and avoid the unwanted UI for image/video capture.  
10.	If at any point, press the lower left-hand side of the screen to repopulate the UI.  
a.	If at any point, lock the Screen Orientation as needed.  
b.	If at any point, turn on Occlusion.  
11.	Once satisfied with the model, press return to model selection to choose another model or close the application.  
![image](https://github.com/user-attachments/assets/b987ffd9-ab46-486f-8558-cddb1eaa8b03)
