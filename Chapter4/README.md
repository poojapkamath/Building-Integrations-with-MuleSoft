# Importing a Shareable Project JAR File into the Cloud IDE
## Overview
This guide outlines the steps to import a JAR file for a Mule project and load it into Anypoint Code Builder within the Cloud IDE.

1. Ensure No Open Projects
Before proceeding, verify that no project is open in the Cloud IDE.

2. Open the Command Palette
You can open the Command Palette using the following methods:
Keyboard Shortcuts:
- Mac: Cmd + Shift + P
- Windows: Ctrl + Shift + P
Menu Navigation:
- Click the menu icon and select View > Command Palette.

3. Open a Folder
Execute the following command in the Command Palette:
File: Open Folder...


- Select your Anypoint Code Builder home directory or any folder outside of a Mule project and click OK.
- If prompted, trust the authors of the files in the directory.
- The IDE will load the selected directory.

4. Import the JAR File
- Drag your shareable JAR file from your computer to the Explorer view in the Cloud IDE.
- If prompted, trust the authors of your file or directory.
- Avoid clicking "Open Anyway" if warned that the file is binary or has unsupported encoding.
- If the folder is large, the IDE will show an upload progress bar—click it to expand.

5. Import the Mule Project
Open the Command Palette again using shortcuts or menu navigation.
Run the following command:
MuleSoft: Import a Mule Project


- Select the shareable JAR file you want to import.
- Choose a destination folder for the unpacked project (such as your home directory or any folder outside a Mule project).
- Click OK to begin the extraction process.

6. Open the Workspace
If your Mule project folder is closed, open a workspace for the project at its root directory.

7. Load Dependencies
- The graphical canvas and dependencies from pom.xml will be loaded.
- If any Mule runtime or Java configuration is missing, set the versions via the canvas.
- Libraries will be loaded into /target/repositories within the project folder.

8. Set Mule Runtime Version (If Needed)
If prompted, click Set Version in the Project Properties tab to assign a supported Mule runtime or Java version.

9. Test Your Project
- Check for errors and ensure the configuration XML and graphical canvas load properly.
- Verify that component dependencies are resolved.
- Adjust ports or file paths in the configuration XML if needed.

10. Run & Debug Your Project
Once everything is set up, run and debug your project using the built-in tools in Anypoint Code Builder.
