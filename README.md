# User Centric Frontend Milestone

Overview:

With this project I've stuck with using the template files supplied regarding a band called "The Monkees". My mentor has set a challenge to try and avoid using bootstrap by using flexbox
and/or other methods to set the stucture out for my website. I've gone for a simplistic design as I had mobile users in mind, so this will load quickly on all devices. I've created 5 pages which include; Index (main), Music, Events,
Band and Contact us. 
 
## UX

I started this project knowing that the website was for a band who want to get better exposure out on the wider web! With this in mind the website needed to feature space for sample tracks, video's,
band info, event line ups and most importantly a way for general public to be able to contact them for hiring. I started out with paper to draw my ideas which I then used a program called 'Pencil' to mock up
a digital version which could be sent so they have an idea of what I was planning to do (documents included). With all this in mind, as a user you can easily and quickly navigate around the site with
no issues.

### User Stories

- I'd like to listen to some music, I click on Music tab and click on play, this will play a track hosted on the site.
- I'd like to view their line up to see where they're playing next, click on the Events tab and look down the Events table, can see where they're playing and purchase tickets.
- I'd like to know who's in the band, click on the Band Tab and scroll down, this will show the band members with an image and description.
- I'd like to book them for an event, click on the contact us page and send a message, this will allow people to contact the band for queries.

## Features

Main Page: When you arrive to the site you're greeted with a vivid background which has an opaque layer over the top, this has quotes as well as a video implemented half way down the page.
Music Page: This page has a solid background colour, music is in a list where a user can hit play and listen without any issues. If they want to purchase any tracks or albums they can do so by 
            clicking on the image directly below the text.
Events Page: This page implements a table to layout the Date, Location and place to purchase tickets via an external source.
Contact Page: This utilises a form with ID's linking the label to the text fields, all having the 'required' tag so each box needs to be filled including @ on email which once done will
              use javascript to send a simple alert saying the message has been sent.
NavBar: Simply links inline when used on a big screen otherwise utilised a checkbox method to make a drop down menu making it quick and easy to navigate around on a small device.

### Existing Features
- NavBar - allows users to navigate by clicking the links at the top. 
- NavBar ~ small screen - Saves space on screen by utilising a checkbox method for a button to bring up the nav menu.
- Video Player - allows user to watch a video with ease by simply clicking on the screen. This has the controls to play, pause, expand and adjust volume.
- Music Player - allows user to listen to a preselected list of tracks by having a list of tracks on the page in an easy to see spot, simply push to play.
- Contact Us Form - allows user to send a message by filling out details and submitting via the submit button.


### Features Left to Implement
- I'd like to have implemented social media live "tweets" or "posts" from facebook, twitter and youtube respectively.

## Technologies Used

- [HTML5] (Intergrated)
    - I used HTML5 for adding content to my web pages.

- [CSS](Intergrated)
    - I used CSS to build the structure for the site instead of bootstrap, set colours, spacing and general manipulation of items on screen.

- [Animate.css](https://daneden.github.io/animate.css/)
    - Used this to make entering a page a little more interesting, avoided using Javascript as some users have this disabled by choice or policy.

- [JavaScript](Intergrated)
    - I used JavaScript to make a message appear on the screen when a form is submitted.


## Testing

In this section, you need to convince the assessor that you have conducted enough testing to legitimately believe that the site works well. Essentially, in this part you will want to go over all of your user stories from the UX section and ensure that they all work as intended, with the project providing an easy and straightforward way for the users to achieve their goals.

Whenever it is feasible, prefer to automate your tests, and if you've done so, provide a brief explanation of your approach, link to the test file(s) and explain how to run them.

For any scenarios that have not been automated, test the user stories manually and provide as much detail as is relevant. A particularly useful form for describing your testing process is via scenarios, such as:

1. Contact form:
    1. Go to the "Contact Us" page
    2. Try to submit the empty form and verify that an error message about the required fields appears
    3. Try to submit the form with an invalid email address and verify that a relevant error message appears
    4. Try to submit the form with all inputs valid and verify that a success message appears.

2. Stream Music:
    1. Go to the "Music" page
    2. Scroll down to the selected track and hit play to which it starts
    3. Press the stop button which halts all music
    4. Click anywhere on the progress bar which skips into the song with no issues
    5. When screen shrinks it also shrinks and is still viewable as well as accessible

3. Events List:
    1. Go to the "Events" page
    2. Scroll down the page to where you'll see a table listing events coming up
    3. Table shrinks and grows with the screen and keeps clarity
    4. Click on the link under "tickets" which takes you to another page, in  a separate window to purchase a ticket

4. NavBar: 
    1. Go to navigation bar at top of website
    2. Scroll accross to make sure all links stay in line
    3. Shrink screen make sure it drops into a dropdown menu when screen becomes too small to fit menu in

5. Images/Content:
    1. Browsing the site in full screen (1080p) making sure content is central and of correct sizes
    2. Shrink screen to iPad resolution checking all sits as it should and nothing overflows
    3. Shrink screen to Phone resolution (Samsung S7) and checking all fits and sits as it should on the page and that the navigation menu changes

6. Different Browsers:
    1. I've tested this mainly in FireFox as that's what I use for my everyday browser using the "inspect" to adjust screen sizes
    2. I've tested this in Chrome as I use this at work to see how it displays the content differently and displays similarly to FireFox in all resolutions
    3. End of project test in Microsoft Edge and confirmed all content is displayed as it was in Chrome and FireFox. Used "Dev Tools" to manipulate resolution

### Issues while building

Whilst building this website I had run across a few problems which are likely from user error. Starting with the Menu when the screen is below X pixels, the inline menu
sets display to 'none' and the checkbox "button" appears but once pressed the menu didn't appear. I found that the translate(y) was telling it to go further out of the 
screen than it already was, meaning it wasn't showing up when the user clicked it.

Images/Video were set with "max-width" or "max-height" expecting the image to get to the set width/height and stop growing in relation to the screen size only to find it
would get to the set height/width and not get any smaller, so would end up taking up the size of the screen in 1080p but in mobile or iPad resolution the image overflowed off the screen.

Band Members was an interesting one as I had orignally wanted to have them aligned with image to the left and all text to the right, it looked great before I intended to change the layout slightly
and ended up having the text staying to the right even when the resolution was set at iPad, it would drift off the screen focusing on the picture which also wasn't going to the set width/height to fit 
the smaller screen size.

"Contact Us Form" I used field set to bulk all the required info into a neat section in the middle of the screen which I quickly learnt meant if you have a user with bad eye site or use software to
read text out load wouldn't actually read the text above the input fields as they weren't linked. Removed the fieldset and re did the form so now the Label have ID matching the input bar meaning read aloud software
can recognise what's there and user can click on the label which will put the focus on the linked input box. While setting up the submit button I linked the JavaScript to the button meaning if no info was entered
it would complain on the screen but also pop up saying the message had sent, even though it hadn't. I sorted this issue and the form acts as you'd expect it to with input fields being checked for input.


## Deployment

This section should describe the process you went through to deploy the project to a hosting platform (e.g. GitHub Pages or Heroku).

I chose to use GitHub Pages to host my project this time around as I had already setup an account while going through this coarse. Big plus was I could commit and push quickly through the terminal in Cloud9 
making it for quick commits.

I started by signing into GitHub Pages, creating a new repositry, set to public (meaning anyone can view but only who I chose can amend/edit).
Cloned my files using terminal in Cloud9 pointing it to my github (git clone https://github.com/99ron/99ron.github.io).
Once this was linked I could "Git add ." to select all my files from root folder and then "git commit -m "Initial upload!" " to set text letting me know what has been done on this commit,
I now needed to push the data onto the GutHub Pages platform now we've made a space, selected what needs to be uploaded and finally upload it to my repositry! I did this by typing into the console
"git push" which then requested my GitHub Pages username and password, which once accepted showed progress of upload.

The way I ran my code was to use the 'run' feature in Cloud9 to open up the website on an external window so I could work on one while checking results on the other.



## Credits

### Content
- The text for section Y was copied from the [Wikipedia article Z](https://en.wikipedia.org/wiki/Z)

### Media
- The photos used in this site were obtained from ...

### Acknowledgements

- I received inspiration for this project from X test
