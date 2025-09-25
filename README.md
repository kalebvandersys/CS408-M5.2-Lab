# Accessibility

This project was introducing accessibility features and allowed me to practice good accessibility practices during website design.

## Development

It is recommended to use the VSCode Live Server extension to run the project locally. There is no need to run a build process or refresh the page manually. Additionally, you do not need to setup a local server to run the project. Please run the live preview, then copy the link and put it in your browser. (After installing the extension, click the name of the project at the top of VSCode, click show and run commands, then type and select "Live Preview:Start Server".)

## Testing

N/A

## Accessibility Lab Answers

Color:

The text is difficult to read because of the current color scheme. Can you do a test of the current color contrast (text/background), report the results of the test, and then fix it by changing the assigned colors? 

The lighthouse test reports "Background and foreground colors do not have a sufficient contrast ratio." before making any changes. It appears to flag ~37 elements. The lighthouse accessibility total score is 85. 
After fixing the lighthouse recommended changes under Contrast, the score increases to 89 and the contrast section in the Lighthouse test is gone.

Semantic HTML:

The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.
I am able to go through the menu, the search field and Go!, the audio clip, and the related links. It does not go to the comments area.

Can you update the article text to make it easier for screen reader users to navigate?
Yes. By adding h1 and h2 headers and <p> tags. Also by removing font elements.

The navigation menu part of the site (wrapped in <div class="nav"></div>) could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update. 
It should be <nav>.

The Images:

The images are currently inaccessible to screen reader users. Can you fix this?
Yes. I added an alt tag to each of the photos that discribe the photo.

The Audio Player:

The <audio> player isn't accessible to hearing impaired (deaf) people — can you add some kind of accessible alternative for these users?
Yes. I added an audio transcript.
The <audio> player isn't accessible to those using older browsers that don't support HTML audio. How can you allow them to still access the audio?
I provided a link to download the audio.

The Forms:

The <input> element in the search form at the top could do with a label, but we don't want to add a visible text label that would potentially spoil the design and isn't really needed by sighted users. How can you add a label that is only accessible to screen readers?
By using the aria-label class.

The two <input> elements in the comment form have visible text labels, but they are not unambiguously associated with their labels — how do you achieve this?
You can add label elements to achive that.

The Show/Hide Comment Control:

The show/hide comment control button is not currently keyboard-accessible. Can you make it keyboard-accessible, both in terms of focusing it using the tab key and activating it using the return key?
I did it by making it a button instead of a div.

The Table:

The data table is not currently very accessible — it is hard for screen reader users to associate data rows and columns together, and the table also has no kind of summary to make it clear what it shows. Can you add some features to your HTML to fix this problem?
Yes. Changing the headers to th helps. Also, adding a caption improves it. Adding the aria aria-describedby provides an overview for screen readers.

Other Considerations?
Can you list two more ideas for improvements that would make the website more accessible?
Yes. One was adding the lang declaration to the html element in the beginning.
Another idea would be to have a show/hide transcript button.

## Sources
https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Reference/Attributes/aria-label#:~:text=Accessible%20names%20can%20also%20be,with%20a%20recognizable%20accessible%20name.