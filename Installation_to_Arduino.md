# How to install Arduino codes on your system
# NOTE: These instructions are being revised to reflect my recently refactored repositories.
Here are (relatively) simple procedures for installing the Arduino codes in my repositories into your own system.  The repositories come in two types, *-library* and *-sketches*; each repository's name will be tagged with one or the other.  If a repository's name has neither, it's not Arduino code.

I know the procedures below look rather involved, but you'll quickly get the hang of them after you've followed along once or twice.

## *-library*
1. Set your browser to the top page for a given repository.  For example, if you want to install the **StateMachine** library, go to page https://github.com/twrackers/StateMachine-library.
2. Click the green **Clone or download** button.
3. When a popup appears by the button, click **Download ZIP**.
4. When prompted, specify where on your system you want the ZIP file to be saved.  This should be somewhere *other* than in your Arduino workspace, for example on your Desktop.  For this example. the file would be named **StateMachine-library-master.zip**.
5. Open the ZIP file.  You should see it contains a single folder.  For this example, the folder in the ZIP file would be **StateMachine-library-master**.
6. Extract the entire ZIP file to a known location.  You will now have a new folder, in this case named **StateMachine-library-master**.
7. Open the new folder.  You will see a **README.md** file (it's readable as text) and the actual library folder, for this example named **StateMachine**.
8. Copy the *entire library folder* into your Arduino workspace's **libraries** folder.  On my Windows 10 system, this is my **Documents\Workspaces\Arduino\libraries** folder.  So on my system, I would end up with a new **Documents\Workspaces\Arduino\libraries\StateMachine** folder.
9. If you had the Arduino IDE running during this last step, you'll need to restart it for the IDE to recognize the presence of the new library.

You can now use your newly installed library in sketches by adding the line

**`#include <StateMachine.h>`    // or whatever the library is named**

to your source codes.

## *-sketches*
1. Set your browser to the top page for a given repository.  For example, if you want to install the **Throttle** sketches, go to page https://github.com/twrackers/Throttle-sketches.
2. Click the green **Clone or download** button.
3. When a popup appears by the button, click **Download ZIP**.
4. When prompted, specify where on your system you want the ZIP file to be saved.  This should be somewhere *other* than in your Arduino workspace, for example on your Desktop.  For this example. the file would be named **Throttle-sketches-master.zip**.
5. Open the ZIP file.  You should see it contains a single folder.  For this example, the folder in the ZIP file would be **Throttle-sketches-master**.
6. Extract the entire ZIP file to a known location.  You will now have a new folder, in this case named **Throttle-sketches-master**.
7. Open the new folder.  You will see a **README.md** file (it's readable as text) and a folder named **sketches**.
8. In the **sketches** folder you'll see one or more folders; these are the actual Arduino sketches.  Remember, an Arduino sketch consists of a folder with the sketch's name, for example **ThrottleTest**, and this folder contains the sketch's actual source file (here it would be **ThrottleTest.ino**) and possibly additional C/C++ header and source files (**`*.cpp`** and **`*.h`** files).
9. Copy the *entire sketch folder* for each sketch you want into your Arduino workspace's **sketches** folder.  On my Windows 10 system, this is my **Documents\Workspaces\Arduino\sketches** folder.  So on my system, I would end up with a new **Documents\Workspaces\Arduino\sketches\ThrottleTest** folder.
10. If you had the Arduino IDE running during this last step, you'll need to restart it for the IDE to recognize the presence of the new sketches.
