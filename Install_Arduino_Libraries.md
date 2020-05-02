# How to install Arduino libraries on your system
Here are procedures you should use to install Arduino libraries from my repositories into your own system.  The library repositories have names ending in *-library*.  If you want to install from the sketch repositories  (names ending in *-sketches*), there's a separate document for that in this *MyDocuments* repository.

The following instructions assume you are running a fairly recent version of the Arduino IDE.  As of 1 May 2020 the current version is 1.8.12, which is what I am running.  At some time in the past year the IDE gained a new feature: installing libraries from ZIP files.  These instructions will make use of that feature.

1. Set your browser to the top page for a given repository.  For example, if you want to install the *StateMachine* library, go to page [https://github.com/twrackers/StateMachine-library](http://github.com/twrackers/StateMachine-library).
2. Click the green **Clone or download** button.
3. When a popup appears by the button, click **Download ZIP**.
4. If prompted, specify where on your system you want the ZIP file to be saved.  (Not every browser prompts the user.)  You should store the ZIP file somewhere *other* than in your Arduino workspace.  On my Windows 10 and Raspberry Pi systems, the default is to save the file in my Downloads folder.  For this example. the file would be saved as *StateMachine-library-master.zip*.
5. From the Arduino IDE menu, click **Sketch -> Include Library -> Add .ZIP Library...**.  A file chooser window will open.
6. Navigate to the folder where you saved the ZIP file, select the file, and click on **Open**.  The IDE should now extract the files from the ZIP file and install them for its use.
7. To verify this worked, again click **Sketch -> Include Library**, then scroll the list of installed libraries until you find the one you just installed.  For this example, the library would be listed simply as *StateMachine*.

You can now use your newly installed library in sketches by adding the line

	#include <*insert libray name here*.h>    // such as <StateMachine.h>

to your source codes.
