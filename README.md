# ios-conv

June 9, 2023

ios-conv is one of many steps in a process I developed to extract notes from an iPhone backup and turn them into a series of discrete plain text files, which I could then feed into [msgen] to create one file I could turn into a published work.

# Usage
Here's the process I developed. It's convuluted...:
1. Download [iTunes Backup Explorer](https://github.com/MaxiHuHe04/iTunes-Backup-Explorer).
2. Extract the `NoteStore.sqlite` file. I was able to find it under Applications and then under `AppDomainGroup-group.com.apple.notes`
3. Download [Apple Cloud Notes Parser](https://github.com/threeplanetssoftware/apple_cloud_notes_parser).
4. Run the ripper program, providing your extracted NoteStore file in the process. See the notes parser README for more information on how to do this.
5. Find the all_notes JSON file in the notes parser program's output directory. Place this in the same directory you saved ios-conv.py into. Rename the JSON file to `inotes.json` and run ios-conv. Doing so will create a notes/ directory containing one text file for every note contained in the NoteStore. 
6. Download [Advanced Renamer](https://www.advancedrenamer.com/)
7. 
