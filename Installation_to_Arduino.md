# How to install Arduino codes on your system
Here are procedures you should use to install the Arduino codes in my repositories into your own system.  The repositories come in two types, *-library* and *-sketches*; each repository's name will be tagged with one or the other.  If a repository's name has neither, it's not Arduino code.

## *-library*
The following instructions assume you are running a fairly recent version of the Arduino IDE.  As of 1 May 2020 the current version is 1.8.12, which is what I am running.  At some time in the past year the IDE gained a new feature: installing libraries from ZIP files.  These instructions will make use of that feature.
1. Set your browser to the top page for a given repository.  For example, if you want to install the **StateMachine** library, go to page https://github.com/twrackers/StateMachine-library.
2. Click the green **Clone or download** button.
3. When a popup appears by the button, click **Download ZIP**.
4. If prompted, specify where on your system you want the ZIP file to be saved.  This should be somewhere *other* than in your Arduino workspace.  On my Windows 10 and Raspberry Pi systems the default is my Downloads folder; not all browsers will prompt you for a location.  For this example. the file would be named **StateMachine-library-master.zip**.
5. From the Arduino IDE menu, click **Sketch -> Include Library -> Add .ZIP Library...**.  A file chooser window will open.
6. Navigate to the folder where you saved the ZIP file, select it, and click on **Open**.  The IDE should now extract the files from the ZIP file and install them for its use.
7. To verify this worked, again click **Sketch -> Include Library**, then scroll the list of installed libraries until you find the one you just installed.  For this example, the library would be listed simply as *StateMachine*.

You can now use your newly installed library in sketches by adding the line

**`#include <*insert libray name here*.h>    // such as <StateMachine.h>`**

to your source codes.

## *-sketches*
1. Set your browser to the top page for a given repository.  For example, if you want to install the **Throttle** sketches, go to page https://github.com/twrackers/Throttle-sketches.
2. Click the green **Clone or download** button.
3. When a popup appears by the button, click **Download ZIP**.
4. If prompted, specify where on your system you want the ZIP file to be saved.  This should be somewhere *other* than in your Arduino workspace.  On my Windows 10 and Raspberry Pi systems the default is my Downloads folder; not all browsers will prompt you for a location.  For this example. the file would be named **Throttle-sketches-master.zip**.
5. Open the ZIP file.  You should see it contains a single folder.  For this example, the folder in the ZIP file would be **Throttle-sketches-master**.
6. Extract the entire ZIP file to a known location.  You will now have a new folder, in this case named **Throttle-sketches-master**.
7. Open the new folder.  You will see a **README.md** file (it's readable as text) and one or more other folders.  Each of these folders contains all the source and header files for a single sketch.  Remember that an Arduino sketch consists of a folder with the sketch's name, for example **ThrottleTest**, and this folder contains the sketch's actual source file (here it would be **ThrottleTest.ino**) and possibly additional C/C++ header and source files (**`*.cpp`** and **`*.h`** files).
9. Copy the *entire sketch folder* for each sketch you want into your Arduino workspace's **sketches** folder.  On my Windows 10 system, this is my **Documents\Workspaces\Arduino\sketches** folder.  So on my system, I would end up with a new **Documents\Workspaces\Arduino\sketches\ThrottleTest** folder.
10. If you had the Arduino IDE running during this last step, you may need to restart it for the IDE to recognize the presence of the new sketches.
