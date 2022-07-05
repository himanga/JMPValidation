# JMP OSI PI Data
This add-in is available in the Add-Ins section of the JMP Community.  Find it here:
https://community.jmp.com/t5/JMP-Add-Ins/Validation-for-Continuous-Processing-Data/ta-p/517689

Source code is available on github:
https://github.com/himanga/JMPValidation

## Building from Source
Run the build.ps1 powershell script.  This builds the documentation files and copies the contents of the AddinFiles folder to a zip file with a .jmpaddin extension.

Title: To Modify this Add-in

About: Developer Dependencies

To make changes to and rebuild this add-in (this is rare), you will also need:

- Natural Docs (program to install)
- jsl-hamcrest add-in for JMP (add-in for JMP, available on community.jmp.com)
- Optional: Add-In Manager add-in for JMP (add-in for JMP, available on community.jmp.com)
- git (program to install)
- GitHub

About: Steps

- Clone git repository
- Make changes
- Document code using natural docs language
- Update and run unit tests
- Use add-in manager to deploy and test dev and versions of add-in or zip files in AddinFiles directory and change the extension to .jmpaddin
- test add-in
- Update documentation (available under the Addins -> ThisAddIn -> Help menu) with a command similar to this in powershell (note the & at the beginning):
  > & "C:\Program Files (x86)\Natural Docs\NaturalDocs.exe" "C:\JMP\JMPValidation\NaturalDocs"

- Use add-in manager to update the version number and deploy prod version of add-in
- Commit changes in git and push commits to github.
- Open a pull request on github

