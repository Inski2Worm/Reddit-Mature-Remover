# Reddit-Mature-Remover
An excel file and a Python file that removes the 18+ age gate on Reddit. You will need Python installed and added to PATH for this to work, and perhaps the Selenium and pyarmor libraries. You will also need Microsoft Excel and you will need to enable the macros. It will say it isn't safe, it's your choice weather you want to trust me or not, I do not care.

HOW TO USE:

I've designed this to be very simple because it really isn't too complex in the first place.

When you first start it will ask to set your directory, follow the very easy instructions there and you should have no issues. (should you encounter any issues however you can manually set it on the sheet in cell B11)

You will be greeted with a very simple UI. Just set Reddit as the URL prefix (I was planning on eventually making this system modular, hence it is a combination box) and then copy the full web address from your address bar (the age-gated address) and then hit run.

If you have the option called "Address Checker Toggle" enabled a messagebox will appearing stating that you have a seemingly correct web address, or if you inputted it incorrectly it will state the opposite.
You can disable this feature in case it has any bugs. (I dobut it will)

The "Quit" button is pretty self explanatory.

The "Run With Shell" toggle is a checkbox that dicates if the python shell will open when you hit "Run". (very helpful option for debugging)

In case you didn't set the directory manually or set it via the script and still attempted to open the application, it will lock every control except for the "Set Directory" button which will re-route you to the directory setting script. (This is so the script doesn't throw an error when it tries to simply find certain files, for example in the images folder.)

You can change the background if you want by going into /Images and changing the background image (MAKE SURE IT'S NAMED THE SAME!!). Please bear in mind I do not know how this will look with certain photos and I will not make a tool that crops it for you.
Another thing to note is that Excel seemingly has a problem with PNG files, just something so you know.

I should also probably let you know in case you do not notice it, but in the ZIP file there is also 2 text files, one is simply a single web address, which is part of the functionality of the script. However, the other is a sort of "browsing history" in a sense, because it logs the web addresses you have visited and the time / date. I'll probably make a feature at some point where you can disable / enable this.

Please let me know if you encounter any bugs, and if you do want to submit a bug report, try running with the "Run With Shell" option enabled and tell me what it says there.

****BY USING THIS TOOL YOU ARE AFFIRMING THAT YOU ARE AT LEAST 18+ YEARS OF AGE AND ARE ONLY DOING THIS SO YOU DON'T HAVE TO CASUALLY LEAK YOUR GOVERNMENT ID ON THE INTERNET.****

**KNOWN BUGS:**
- There is no system to handle if elements are not found, occasionally leading to the browser to close out randomly because it couldn't find things. (Probably quite rare, but I'll add a system for it nonetheless)
