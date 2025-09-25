# Accessibility on A Web Page - CS408 Lab5

This is a lab that acts as an excersise in maintaining accessibility when making a web page. The Lab covered a project built with plain HTML and CSS rules, and the objective was to transform the initial web page into something that is more accessible. The target groups to consider were keyboard-only users, screen-reader users, and people who have poor vision.

REMEMBER LOOKING UP LABEL TAG!

## Getting Started

To get started, clone this repository and open the HTML file in your browser.
There are no dependencies or anything else that need to be downloaded.

## Development

It is recommended to use the VSCode Live Server extension to run the project
locally. It is also incredibly useful because it lets you open a LocalHost server to see the website as intended and not as a preview to the side. As it updates automatically, there is not need to refresh the page multiple times to see the changes.

## Testing

There are not really any tests to run here, so there is no need to run any specific commands.

## Accessibility Lab Answers

### Color

I put the two colors #2a2a2a and #008000 into a website that rates the contrast between two
and it recieved a poor score of 2.79 : 1. According to <www.webaim.org/resources/contrastchecker/>:
a contrast ratio of 4.5:1 for normal text, 3:1 for large text like headers and for graphics.
Keep in mind that that was the less strict test. Upon changing the background to white ( #FFFFFF )
the score shot up to 14.35 : 1, which is MUCH better.

### Semantic HTML

1. When trying to navigate the website using the keyboard (AKA, pressing tab to navigate by keyboard), the highlight only appears on the HOME tab and pressing any arrow key
does not move it at all. Pressing the left and right arrow key should move the highlight, but pressing up and down does scroll up and down the page. Pressing Tab over and over againdoes move the selector around though! Pressing space rapidly scrolls down the page.

2. Yes, I can update the article text to make it easier to read. Most of that was accomplished by replacing some weirdly formatted tags in the CSS with proper ones. For instance, replacing the "font size = 6" with the tag h2 and such. That corrected the formatting and made it look much closer to what is presented on the example image. I also added < p > tags around the main body text to properly format it and it made things much easier to read through.

3. The < nav > tag ended up being the best fit to replace the div with a class of "nav". It was made specifically for a navigation bar and so it only made sense.

### The Images

I wasn't too sure what we could do for the images that wasn't already avaiable, but it seems like adding and alt to the image to describe what was going on in the image.

### The Audio Player

1. To make it accessible to deaf users, I added a transcript to the bottom of the audio player.
This should let them read along if they so choose.

2. I don't know if it will show up at all, but I added a link in the audio tag that links to the mp3 file for the audio. Through that they shoulld be able to directly download the ausio and play it
for themselves if they want.

### The Forms

1. To make a tag that is only visible to screen readers, I made a new tag .screen_reader to make an invisible lable tag that reads "Search". I think this should work.

2. For this one, we did the same thing we did in the first one, make a tag for both the boxes and associate it with the boc using the pre-made id names. This time, they are not going to be invisible since we want to see them. I also tried to style them like the standard text in the main body.

### Show/Hide Comments Control

As it turns out, the show/hide comments button can be made accessible to keyboard users by changing the tag it was using from a div to a proper button. Upon changing that, when pressing tab the index will highlight the button and make it selectable. I also used the cursor attribute to change how the mouse looks when hovering over the button. After adding the right path to the js folder, the button now works properly with both mouse cursor and the keyboard navigation.

### The Table

To assist in the table's readability, I made use of a tag I saw in the table section of the CSS called "scope='col'". Considering that was in the table section, I assumed that the associated CSS was for making a distinct colunm for the table and was proven correct after seeing how it changed the table's look. I also added some extra CSS to make the rows more defined in the table and it looks like it helped. For the summary, I added a caption to it that described in very broad terms the talking points brought up. By broad terms, I mean the columns since I figured that was importiant to know.

### Other Considerations

Some of the other consideration I chose to do was adding more distinct features to the table to make it more distinct. I think that maybe having a button to increase the font size if needed would help out in case the current size isn't enough. Nothing to wild, maybe a set range or 3 pre-determined options. If I had more time I would definitely try to consider chaning the colors around more to see if there is something there with a nice contrast that still manages to look more interesting than "black text on white background".

## Citations

Not a lot here this time, as I was able to piece together a lot of what I had to do via the provided CSS and such. I did have to look up one though, so here it is.

HTML Label Tag. https://www.w3schools.com/tags/tag_label.asp. Accessed 24 Sep. 2025.
