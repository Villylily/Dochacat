# Dochacat:3
"Dough-Cha-Cat"
A Chat interface for Google Docs for when Google Chat is not an option. 
Its also pretty simple to use 
<img width="4754" height="2523" alt="1000000254 (1)" src="https://github.com/user-attachments/assets/9eb553cc-0bd3-437a-92f2-908079abf284" />

# Test Doc to test it out (V9 Pre) ([Click me](https://docs.google.com/document/d/19Txx1OX9DEmWJttRqnpS9llk_ZkHyW_0tyYAGJGMIDI/copy))
How to use

# Setup Instructions
Step 0: The Spreadsheet
Make a copy of this ([Example Sheet](https://docs.google.com/spreadsheets/d/1I1DdL6mkeI2dVKC2NwRVC3PUkyxkwhhHP7J3HBBrdjU/copy)).

WARNING: You must set the Share settings of this sheet to "Anyone with the link, are editors",otherwise the chat will not be able to sync messages.

Step 1: Prepare the Google Doc
Open the Google Doc where you want the chat to appear. Ensure that all users who need to use the chat are added as Editors in this document.

Step 2: Open Apps Script
In your Google Doc, go to Extensions > Apps Script.

Step 3: Configure Code.gs
Ensure the Code.gs file is completely blank. Paste the contents of the DochacatV10_GS.code.txt file into Code.gs and save.

Step 4: Create the HTML File
Click the + (plus icon) next to Files, select HTML, and name it Chat. (Note: Do not include the .html extension in the name, just name it Chat).

Step 5: Paste HTML Code
Paste the contents of the DochacatV10_html.txt file into your new Chat.html file and save.

Step 6: Final Configuration
Go back to Code.gs and follow any remaining internal code comments/instructions (such as pasting your Spreadsheet ID, admin emails).

Step 7: Deploy as a Web App (Optional only needed if you wanna use the full screen modes)  
Click Deploy > New Deployment.

Select Web App as the type.

Add a description (e.g., "Dochacat V10").

Execute as: Me.

Who has access: "Anyone with a Google Account" (or "Anyone within your School Name" for school-specific use).

Click Deploy, authorize permissions, and copy the Web App URL. This URL is your fullscreen chat page.

# FIRST TIME SETUP THESE STEPS MUST BE DONE FOR ALL USERS BEFORE THEY CAN USE THE FULLSCREEN OR DOCHACAT:3
Find the Sidebar: Refresh your Google Doc. Look at the top menu bar (where it says File, Edit, View).
Look for "Dochacat:3": Dochacat:3 will appear to the right of "Help." Thats how you use the sidebar and setup as well 

When you try to open the sidebar for the first time, Google will try to stop you. You must do this in the Google Doc before the Fullscreen link will work right and to use Dochacat:3.

The "Authorization Required" Box: * When you click the Dochacat menu in your Doc, a box will pop up saying "Authorization Required."

Click Continue.

The "Safety" Warning: * A screen will say "This app isn't verified." Don't panic.

Click the small word "Advanced" at the bottom.

Click "Go to Dochacat (unsafe)" at the very bottom. (It’s only "unsafe" because you just made it yourself!)

The Final "Allow": * A list of permissions will show up. Scroll to the bottom and click Allow.

The Popup Blocker: * If the sidebar still doesn't open, look at the right side of your browser's address bar.

If you see a red 'X' icon, click it and select "Always allow popups from docs.google.com."
How to Use
Once deployed, refresh your Google Doc. Dochacat:3 will appear in your top toolbar.

# Auto Open sidebar 
If you want the Sidebar to open automatically when someone opens the Doc, you have to set up a Trigger.

In your Apps Script page, look at the left sidebar and click the Alarm Clock icon (Triggers).

Click the blue + Add Trigger button at the bottom right.

Set the settings exactly like this:

Choose which function to run: showSidebar

Choose which deployment should run: Head

Select event source: From document

Select event type: On open

Click Save.

Google will ask for permission again. Allow everything.

To see a list of commands, simply type /help in the chat box.
