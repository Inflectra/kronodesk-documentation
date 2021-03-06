# Deploying to GitHub Pages
In the master branch, run `mkdocs gh-deploy` and that's it! Your changes should be live after the command finishes!

# Converting docx to MD
1. Install mkdocs with `pip install mkdocs`, if you haven't already. Note that you need [pip](https://pip.pypa.io/en/stable/installing/) and Python for this to work. 
2. [Install Pandoc](https://pandoc.org/installing.html)
3. In the tools directory, paste the .docx files you would like to convert. Note that only .docx files will be converted - if you have a .doc or another format, either save it as a docx or convert it manually
4. In a shell, `cd` to tools and run `python .\spiraconvert.py options` where options is either 'auto' (`python .\spiraconvert.py auto`) or the names of the files you would like to convert without the file extension (`python .\spiraconvert.py "SpiraTestPlanTeam IDE Integration Guide" "SpiraTestPlanTeam External Bug Tracking Integration Guide" "SpiraTest-Team Automated Testing Integration Guide"`)
5. The script will run, copying iles into the `./temp` folder in the root directory as it goes. These markdown files and the images should be pasted into the `./docs` directory in the apropriate folders.
6. Review the files for weirdness (more information below)
7. Put all the new files in mkdocs.yml where you would like. The `nav` property will generate the top navbar in the structure you define. Run `mkdocs serve` to test it out, which can be viewed at http://127.0.0.1:8000/


## Conversion Problems
- Table formatting is generally a huge pain and needs to be done manually
- Code usually isn't formatted and generally has excessive escape characters (I just pasted the code directly from word as it was easier)
- The script will spit out an uneccesary `Introduction` or `Legal` file if it was present or put a legal notice in the `.md` file who's corresponding section in the word file was at the bottom of the word file.
- Unnecessary escape characters: Just do a find and replace in your editor of choice in the `docs\` directory with the criteria below:
    - \\< to <
    - \\> to > **IFF THE OCCURANCE IS IN A CODE BLOCK, OTHERWISE NECESSARY** 
    - \\" to "
    - \\' to '
    - \\@ to @
    - ^®^ to <sup>®</sup>
    - ^1^ to <sup>1</sup>
    - \$ to $

# Delete Unused Pictures
From the tools directory, run the command `python .\unusedimgs.py`. This will generate a list of commands you can paste into the console to delete the file. ***PLEASE READ LIMITATIONS BEFORE YOU PROCEED AND DELETE IMAGES***
## Limitations
- If an image name has a parenthesis in it (like `Importing_from_Microsoft_Excel_(Office365)_24.png`), the script will print it out no matter what. Please review them before you delete in case they are actually used.
- If the image reference is across multiple lines (like the example below), the image will be printed out. Please move the reference to one line and run the command again and it should disappear.

```
...

![Git stores data as snapshots of the project over
time.](img/Using_Git_47.png)

...
```