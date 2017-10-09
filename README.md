# Screenshot to Yoink
This is a simple [Alfred](https://www.alfredapp.com) script that captures screenshots directly into the Yoink app. This was inspired by the [Automator workflow from the Yoink blog](https://eternalstorms.wordpress.com/2015/01/15/capture-selective-screenshots-in-yoink/ "Capture Selective Screenshots in Yoink with Automator"), and the functionality is fundamentally the same. Using Alfred however, is quite a bit faster than using Automator.

## Download
[**Download the .alfredworkflow file**](https://github.com/Irvel/screenshot-to-yoink/blob/master/screenshot-to-yoink.alfredworkflow?raw=true)


### Activating the Workflow with a keyboard shortcut 
![Selective Screenshot Keyboard](https://user-images.githubusercontent.com/2577338/31323684-e2b1b7d0-ac70-11e7-9eda-aaafa80d486e.gif)

### Activating the Workflow with keyword 
![Selective Screenshot Keyword](https://user-images.githubusercontent.com/2577338/31323701-1ae0dafa-ac71-11e7-8590-3e58bc4e601e.gif)

 

### Screenshot name and location
I tried to replicate the default macOS screenshot naming and location. If you've set a custom location via:
```
defaults write com.apple.screencapture location ~/Path/to/Screenshots
```
The script will use that location. If not, it will default to ~/Desktop.  

Additionally, you can set a different screenshot location for this script only via the Alfred Workflow Environment Variable ```screenshot_alt_dir```.


### But what is Yoink and what is Alfred
[Yoink](https://eternalstorms.at/yoink "Yoink Website") is a persistent Drag and Drop shelf utility and [Alfred](https://www.alfredapp.com) is a customizable Spotlight replacement that can run scripts and many other things.


 
 
### Tips and tricks
#### Workflow Shortcut
⇧⌘4 is the default macOS shortcut for saving a screenshot of a selected area and ⇧⌘3 is the default for full-screen. However, you might not want to send every screenshot you take to Yoink. ⇧⌘5 for selective screenshots and ⇧⌘6 are good shortcut alternatives for triggering this workflow:

![Cool Screenshot Shortcuts](https://user-images.githubusercontent.com/2577338/31323716-5963401a-ac71-11e7-92b2-a968c0044e1e.png)

#### Screenshot filename
Simplify the name by removing spaces and just using the unix timestamp:
![Filename alternative](https://user-images.githubusercontent.com/2577338/31323734-88b7c0f2-ac71-11e7-94aa-55a68e613363.png)
