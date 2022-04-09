# How to add Visual Studio Code shortcuts into macOS Finder:

1. Launch Automator

2. Create New Document

3. Create a new Quick Action Select "Quick Action"
![alt text](https://i.stack.imgur.com/BwWGs.png "Quick Action")

4. Add the Action...
* Workflow receives current **files or folders** from **Finder.**
* Add a new Run Shell Script action to the workflow. (drag the "Run Shell Script" object, highlighted in the screenshot, to the empty window on the right)

5. Configure the Workflow
* Set the Pass Input to be **as arguments**
* Paste the following in the input box:
```open -n -b "com.microsoft.VSCode" --args "$*" ```
![alt text](https://i.stack.imgur.com/MnPT6.png "Workflow")

6. Save the action using a name like **Open In Visual Studio Code.**

You may now *right-click* on the folder and find your newly created task under **Quick Actions.**

![alt text](https://i.stack.imgur.com/0VeSP.png "Quick Actions Final")