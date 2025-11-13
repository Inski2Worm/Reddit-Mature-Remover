# Reddit-Mature-Remover
An excel file and a Python file that removes the 18+ age gate on Reddit. You will need Python installed and added to PATH for this to work, and perhaps the Selenium and pyarmor libraries. For the best experience you will also need Microsoft Excel and you will need to enable the macros. It will say it isn't safe, it's your choice weather you want to trust me or not, I do not care.

Are you tired of feeling violated for simply browsing the internet?

Tired of having to submit your ID to sketchy 3rd party providers with very loosely defined policies?

Well here is a small little act of rebellion against it! This only works on Reddit as of current, and probably for the forseeable future, however the fact that it works is still nice right?
Microsoft Excel is the reccommended version that you should use as I have years worth of experience with VBA whereas with LO Basic I have barely any, more is explained below!

**GET THE LATEST VERSION BY CHECKING TAGS!**

# HOW TO USE:

I've designed this to be very simple because it really isn't too complex in the first place.

- When you first start it will ask to set your directory, follow the very easy instructions there and you should have no issues. (should you encounter any issues however you can manually set it on the sheet in cell B11)

- You will be greeted with a very simple UI. Just set Reddit as the URL prefix (I was planning on eventually making this system modular, hence it is a combination box) and then copy the full web address from your address bar (the age-gated address) and then hit run.

- If you have the option called "Address Checker Toggle" enabled a messagebox will appearing stating that you have a seemingly correct web address, or if you inputted it incorrectly it will state the opposite.
You can disable this feature in case it has any bugs. (I dobut it will)

- The "Quit" button is pretty self explanatory.

- The "Run With Shell" toggle is a checkbox that dicates if the python shell will open when you hit "Run". (very helpful option for debugging)

- In case you didn't set the directory manually or set it via the script and still attempted to open the application, it will lock every control except for the "Set Directory" button which will re-route you to the directory setting script. (This is so the script doesn't throw an error when it tries to simply find certain files, for example in the images folder.)

- You can change the background if you want by going into /Images and changing the background image (MAKE SURE IT'S NAMED THE SAME!!). Please bear in mind I do not know how this will look with certain photos and I will not make a tool that crops it for you.
Another thing to note is that Excel seemingly has a problem with PNG files, just something so you know.

- I should also probably let you know in case you do not notice it, but in the ZIP file there is also 2 text files, one is simply a single web address, which is part of the functionality of the script. However, the other is a sort of "browsing history" in a sense, because it logs the web addresses you have visited and the time / date. I'll probably make a feature at some point where you can disable / enable this.

Please let me know if you encounter any bugs, and if you do want to submit a bug report, try running with the "Run With Shell" option enabled and tell me what it says there.

# LIBRE OFFICE VERSION ADVISORYS:

- The LibreOffice version functions in very much the same way as the Excel version. However some features are literally just not working. I cannot for the life of me get the Shell to simply run a simple python script meaning it must be manually ran from the project directory. I've tried to make it as easy as possible, but it's still annoying to me that it doesn't work.. for now. 

- Because you literally cannot run the python file from the script the "Run With Shell" option is greyed out.

- The UI looks terrible for now because it was put together with functionality over looks, I will improve it to look like the Excel one in the somewhat near future. Excel remains my primary area of development.

- Code will error out upon first pressing the open button. It's okay, it  will work the second time, just re-run it. I'm fixing this in a planned bugfix patch.

# MISC:

****BY USING THIS TOOL YOU ARE AFFIRMING THAT YOU ARE AT LEAST 18+ YEARS OF AGE AND ARE ONLY DOING THIS SO YOU DON'T HAVE TO CASUALLY LEAK YOUR GOVERNMENT ID ON THE INTERNET.****

**KNOWN BUGS:**
- There is no system to handle if elements are not found, occasionally leading to the browser to close out randomly because it couldn't find things. (Probably quite rare, but I'll add a system for it nonetheless)
- Loading a page that only contains a video / photo as opposed to an actual subreddit or just a user has a slightly different blocking element so I need to script that in.
    - Update(06/11/2025: 04:33): I have found the element that does this and will work on scripting it in tomorrow.
    
    - Update(08/11/2025: 00:01): I had actually not found what I needed to adjust, but I have now found it. Will start actual scripting tomorrow.

**PLANS:**
- MAYBE learn LibreOffice Basic code to port over all my VBA functions as best as I can so people have an alternative to using MS Excel. (because Excel is paid)
  - Progress:
  
    I am currently porting over my code from VBA to LO Basic (LibreOffice Basic), the libraries are very similar and they both function relatively similar, however some things are obviously still requiring tweaking. For example, there is an issue where the shell just        refuses to run the python file, I'll need to learn more about the language to understand what is going on there. Side note: The UI currently looks terrible because I had to remake it as LO doesn't support .frm files.

    Progress as of 05/11/2025 22:06; I have made a functional version of the code. Shell still doesn't run python script. Still working on it.

    Progress as of 06/11/2025 04:25; I have uploaded an incomplete version of the LibreOffice application in hopes of improving it in the future.

    (All times provided are in GMT)

**Changelog:**
- Added an age affirmation prompt within the app itself.
