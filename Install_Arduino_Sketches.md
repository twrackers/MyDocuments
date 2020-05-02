# How to install Arduino sketches on your system
Here are procedures you should use to install Arduino sketches from my repositories into your own system.  The sketch repositories have names ending in *-sketches*.  If you want to install from the library repositories  (names ending in *-library*), there's a separate document for that in this *MyDocuments* repository.

1. Set your browser to the top page for a given repository.  For example, if you want to install any of the *TrackSensor* sketches, go to page [https://github.com/twrackers/TrackSensor-sketches](http://github.com/twrackers/TrackSensor-sketches).
2. Click the green **Clone or download** button.
3. When a popup appears by the button, click **Download ZIP**.
4. If prompted, specify where on your system you want the ZIP file to be saved.  (Not every browser prompts the user.)  You should store the ZIP file somewhere *other* than in your Arduino workspace.  On my Windows 10 and Raspberry Pi systems, the default is to save the file in my Downloads folder.  For this example. the file would be saved as *TrackSensor-sketches-master.zip*.
5. Open the ZIP file.  You should see its contents include one or more folders.  For this example, there are 2 folders in the ZIP file, named *TrackSensor\_Master* and *TrackSensor\_Slave*.  Each of these folders is a separate sketch, containing the sketch's main source file (*.ino*) and possibly additional source (*.cpp*) and header (*.h*) files.
6. Extract the entire ZIP file to a known location.  The easiest choice is usually the default one, to extract into the same directory where the ZIP file is already located.  You will then have a new folder, in this case named *TrackSensor-sketches-master*.
7. Navigate into the new folder.  For each of the sketches you want to use, copy *the entire sketch folder* for each sketch into your Arduino workspace's *sketches* folder.  On my Windows 10 system, that would be my *Documents\Workspaces\Arduino\sketches* folder.
8. If you had the Arduino IDE running during this last step, you may need to restart it for the IDE to recognize that you've loaded new sketches.
