# d3bugging

## Tools: What you need

###  Browser

#### Chrome

- Chrome is great for this.  __Developer Tools__
- Chrome Developer Tools at https://developers.google.com/chrome-developer-tools/docs/scripts-breakpoints
- This guides covers the entire developer tools http://www.codeproject.com/Articles/273129/Beginner-Guide-to-Page-and-Script-Debugging-with-C
- Lots of extensions/resources

#### Safari

- Safari has lot of the same developer functionality as Chrome (They're both WebKit), but presented differently.  
- Developer Mode Must be turned on manually from Preferences -> Advanced
- The UI is similar to Xcode, so you have to dig for things (like stopping on uncaught exceptions)
- It is missing some cool features that Chrome has (like local modifications)

#### Firefox

- I don't generally use Firefox.  Firebug was the dominant debugger tool for years.
- Most of the same debugging functionality as the WebKit browsers 
- They also have a 3D inspector that works with SVG.  Not specifically javascript related, but cool nonetheless.

### Editor

- Text Editors (BBEdit, SublimeText, vi, emacs, really anything)
- IDEs ([JetBrains](http://sites.duke.edu/software/2012/11/19/free-classroom-license-now-available-for-jetbrains-ides/): WebStorm, PyCharm, RubyMine, etc.)
    - Win, Mac, Linux
    - Duke has these licensed for classroom use

### Server/Hosting

- `python -mSimpleHTTPServer`: easy local webserver at http://localhost:8000.
- If you load files or data from a outside of your code, you need to have it on a web server of some kind.
- The python method lets you edit files locally without uploading to a server or installing/configuring apache
    - Save, reload, repeat.
- Gist / bl.ocks.org.  Easy to share/show someone, like these examples

## D3bugging Exercises

### Simple Debugging

[Bar Graph View](http://bl.ocks.org/Leehro/raw/5263797/)

1. Launch Developer Tools, JavaScript Console
2. Chrome will let you edit javascript IN place if it's in a separate JS file (and not just in a script tag)
3. These get lost if you reload the page but would work in a function or a handler

### More complicated Debugging

__Need an example__

![Breakdance point](http://upload.wikimedia.org/wikipedia/commons/thumb/0/00/Break_dance.svg/256px-Break_dance.svg.png)

1. Set a Breakpoint (Standard, Conditional, Fancy)
2. Inspecting values (Local, Global, Watch Expressions)
3. Console to evaluate expressions

### Layouts, external data

Link.

1. Pause on uncaught is your friend! (Purple Stop Sign).
2. Call Stack
3. Bad data?  Be careful.
    - Now I've left a , off my json file on line 409.  Chrome reports it as the .html file.
    - JSON Validator: http://jsonlint.com
