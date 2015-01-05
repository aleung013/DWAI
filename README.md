DWAI
============

###Group Members:
- Alvin Leung: Canvas
- Vivian Wang: Back-end
- Michele Lin: Middle-end
- Judy Mai: Front-end

###How to Run:
Currently deployed at: http://softdev-server.stuycs.org:9001/
Our home page has a bit of an issue with image-retrieving, so please head on to /register or /login to start.

###Project:
Our project, temporarily dubbed Google Paint, was intended to be a version of Google Docs for artists. Multiple artists could collaborate on a drawing simultaneously, while having most of the basic features of more complex graphics programs available to them.
Although we do not yet have multi-person functionality working, we have a canvas that allows users to drawing, change their pen size and color, as well as undo and redo their strokes. Each user also has a gallery that lets them view images they have saved.
For future prospects, we plan on implementing chat and view/edit settings as well as an option to automatically post to social networks such as Facebook, Tumblr, deviantART, etc. 


###Things to work on
1. multi-user chat functionality using node.js and socket.io 
2. update canvaspg with other paint uses: eraser, fix save, consider adding an File-save thing and a change canvas size
3. update profile page and allow user to customize settings to post to Facebook, Tumblr, etc. with something similar to oauth-google
4. see how we can get multiple users adding in a stroke (check out the server stuff and how we will only be doing the undo/redo stuff to the user who made them, not to the entire canvas and not undoing/redoing other people's stuff.
5. think about new animations and site navigation that will make the site more interactive and interesting

###Bugs I'm noticing & Things we need to fix/add & Most current updates
- Individual image page isn't working/doesn't exist. Remember to add an edit/update button as well as a place for an option description. Comments maybe. Also favorites? Stars? Upvotes?
- Chat is still in the making (username stuff...etc), would be cool if it worked
- Home page isn't working?? Google Paint logo should suffice, don't need 'home' on the navbar, that's redundant.
- Need to either distinguish between profile/gallery or just make them the same thing (probably distinguish)
- Padding for the bottom credits is kinda buggy, only works on About page with a quick look
- Dropdowns are consistently giving me trouble. Only work on About/Chat page, not on canvas/profile
- If user is already logged in, Login/Register should no longer be options, just Log out. On a smaller note, be consistent with Login/Logout or Sign in/Sign out.
- Canvas and home are in pretty bad shape. 
   1. Canvas: dropdown for tools isn't working, as are the other dropdowns on the page. undo/redo don't work. Need to make the title after saving actually work. (need to get saving to work period.) Also zoom is just there for show right now.
   2. Home: just giving an outright error msg right now saying 'img' is undefined

- Quick fixes:
   1. Clicking on the user's name should automatically bring to profile (just make it an a href)
   2. Add an "add artwork" button on the profile/gallery pg.
   3. Add more things to profile: "About me", etc. 
   4. "Edit profile" button should really be "Settings"
   5. "Last edited on..." time is missing. Remember this time should update with each update of the drawing (description, etc)
   6. Individual image page should bring up a modal? A separate page would probably be better because then we can add comments and descriptions. If no comments then modal would be better because we can do left/right to other drawings.
   7. Add a little star thing to the top corner of images for a quick starred/favorites.
   8. On that note, add a favorites page.
