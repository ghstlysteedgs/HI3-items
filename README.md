# HI3-items
Horse isle 3 tools that DO NOT interact with the game. Only reads the inputs from your computer, stored locally if you wish. 

How to use:
- **On Windows**:
    - Right click the `.exe` file and "run as administrator" to run it.
    - Depending on the User Account Control settings, Windows may give a warning message like: _"Windows protected your PC."_ This is normal for non-signed applications.
    - To proceed:
        1. Click "More info" in the warning dialog.
        2. Click "Run anyway."
     
  MosiClickCounter was made by Ghostly Steeds Game Studios, this application does not do anything to the horse isle game. It only reads keybind inputs from your computer.

**MosiClickCounter** is a graphical application designed to keep track of mouse clicks while supering and also has a manual counter for each mutation you super past.

### **Features Overview**
1. **Mouse Click Counter**
2. **Item Tracker**
3. **Control Buttons (Start, Pause, Resume, Stop)**
4. **Save Statistics to File**
5. **Graphical Interface**

### **Feature Details**
#### **1. Mouse Click Counter**
The application continuously monitors mouse clicks when active. This feature is useful for tracking the number of times your mouse is clicked after you hit "Start", displaying how many times you click your mouse while navigating through the game.
- The total **click count** is displayed prominently in the interface.
- The click count updates in real time as you interact.

#### **2. Muti Tracker**
The application includes pre-configured mutation counter for tracking how many times you come across each mutation type. Each mut can be updated individually using **+** and **-** buttons to add or remove counts.
    - `Flash`
    - `Birdcatcher`
    - `Grease`
    - `Mosaic`
    - `Tetrarch`
    - `Lace`

- For each item:
    - Clicking the `+` button increases the count by one.
    - Clicking the `-` button decreases the count by one (cannot go below 0).
    - Real-time updates of item counts are displayed.
    - THIS IS NOT DONE AUTOMATICALLY, THIS APP HAS NO WAY TO READ WHAT HORSE ISLE COMES ACROSS.


#### **3. Control Buttons**
MosiClickCounter includes buttons for controlling the session. These buttons allow you to easily manage the behavior of the program.
##### **Start Button**
- Initializes the application and starts monitoring mouse clicks.
- Resets all counters to zero when the session starts.

##### **Pause/Resume Button**
- Toggles the mouse click tracker between **pause** and **resume** states without resetting the counters.
- When paused, all counting stops but remains open for resumption.

##### **Stop Button**
- Stops the session completely and resets **all counters** to zero, including mouse click counts and item counts.
- A confirmation dialog requires you to confirm before resetting.

#### **4. Save Statistics to File**
Users can export their current click and item statistics to a `.txt` file for documentation or record-keeping purposes.
- **How it works**:
    - Click the "Save Stats" button.
    - This opens a dialog box where you can select where the `.txt` file will be saved.
    - The saved file will include:
        - Total number of mouse clicks.
        - The counts for each muti being tracked.

- **Example Output**:
``` 
  Mouse Clicks: 150

  Item Tracker Stats:
    Flash: 5
    Birdcatcher: 3
    Grease: 0
    Mosaic: 1
    Tetrach: 7
```
#### **5. Graphical Interface**
The application features a simple, user-friendly graphical interface made with Tkinter. The design is minimalistic and functional, focusing on usability.
- **Main Components**:
    - A title banner at the top to indicate the application's name.
    - A large display for showing the mouse click count in real-time.
    - A section for item counter displays with clear labels and buttons.
    - Buttons for all main controls: Start, Pause/Resume, Stop, and Save Stats.

### **How to Use MosiClickCounter**
1. **Launch the Application**:
    - Double-click the `.exe` file to launch the program.
    - Give MosiClickCounter a moment to open.
    - A graphical interface will open.

2. **Start Tracking Mouse Clicks**:
    - Click the "Start" button to begin tracking your mouse clicks.
    - Mouse clicks will be counted and displayed in real-time.

3. **Manage Muti Counters**:
    - Use the **+** and **-** buttons next to the items to adjust their count based on your tracking needs.
    - The mutation counts are updated live in the application.

4. **Pause and Resume the Counter**:
    - Click "Pause" to pause tracking without resetting any counters.
    - Click "Resume" (same button) to continue tracking.

5. **Stop and Reset All Counters**:
    - Click "Stop" to stop the click tracker and reset **all counters** to zero.
    - A confirmation dialog will appear to ensure you wish to reset everything.

6. **Save Statistics**:
    - Click "Save Stats" to export the current click count and muti tracker stats.
    - Choose a location and filename to save the `.txt` file.

### **Error Handling and Warnings**
1. **Invalid Actions**:
    - Clicking "Pause" or "Stop" when the counter is not running will display warnings like:
        - _"The counter is not running."_

    - Decreasing an item’s count below zero is not allowed; a warning, _"Item count cannot be negative,"_ will appear.

2. **Confirmation Dialogs**:
    - The "Stop" button triggers a confirmation dialog to avoid accidental resets: _"Are you sure you want to stop and reset the counter?"_

3. **Save Stats Warning**:
    - If there is nothing to save yet, clicking "Save Stats" will display a warning: _"Nothing to save yet, start a session first!"_

### **Technical Details**
- **Platform**: Windows (supports `.exe` format created with PyInstaller)
- **Dependencies**:
    - Python 3+
    - Tkinter
    - pynput (for mouse click tracking)

- **Output**: Saves statistics as a `.txt` file.


4. **Session Analytics**:
    - Add an option to display graphs or trends for the click data over time.

Feel free to share this documentation guide with your users or adapt it as needed! Let me know if you’d like further refinements. 😊

