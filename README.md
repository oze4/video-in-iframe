# video-in-iframe
POC - auto play/pause video tag that lives in an iframe when the page is not visible.

The issue we had was the iframe and video inside of it were not created upon document ready/load. Had to come up with a way to wait for certain elements to be created first before initializing the Page Visible API.

The [Page Visible API](https://developer.mozilla.org/en-US/docs/Web/API/Page_Visibility_API) is how we pause the video when a user switches browser tab, or minimizes the browser, and how we resume playing the video once the tab is 'active' again.

[Why this POC was built to begin with](https://stackoverflow.com/questions/59516224/play-pause-vimeo-video-when-watcher-switches-browser-tab-or-minimize-browser-w/)
