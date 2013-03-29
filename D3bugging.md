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

### Other Tools

1. [JSFiddle](http://jsfiddle.net)
2. [JSLint](http://www.jslint.com), [JSONLint](http://jsonlint.com)
3. [Postman - REST Client](https://chrome.google.com/webstore/detail/postman-rest-client/fdmmgilgnpjigdojojpjoooidkmcomcm)

## D3bugging Exercises

1. Make it work
2. Make it right
3. Make it fast

(loosely)

### Make it work

- View->Developer Tools->JavaScript Console will show syntax errors and uncaught exceptions

### Make it right

![Breakdance point](http://upload.wikimedia.org/wikipedia/commons/thumb/0/00/Break_dance.svg/256px-Break_dance.svg.png)

- Manual breakpoints, conditional, and from code
- Pause on uncaught! (Purple Stop Sign).
  - Be careful with bad data
- Inspecting values
- Call Stack
- Console logging

### Make it fast

- Profiling
