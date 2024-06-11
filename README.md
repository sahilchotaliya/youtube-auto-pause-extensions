# youtube-auto-pause-extensions
# Loading the Extension in Chrome
Open Chrome and go to chrome://extensions/.
Enable "Developer mode" by toggling the switch in the top right corner.
Click on the "Load unpacked" button and select your project directory (youtube-auto-pause).


# Testing the Extension
Open YouTube and start playing a video.
Switch to another application (like VS Code).
The video should automatically pause when the browser tab is not visible.
Switch back to the YouTube tab; the video should resume playing.

# Notes
The background.js script ensures that the content script (content.js) is injected into YouTube video pages whenever a tab is activated or updated.
The content.js script listens for the visibilitychange event to pause and resume the video based on the tab's visibility.
This complete setup should help you create a Chrome extension to automatically pause YouTube videos when switching away from the browser.
