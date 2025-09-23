# web-dev-starter

This is a starter project for web development with no frameworks and minimal
dependencies. It is intended to be a starting point for web development projects
that are written in plain HTML, CSS, and JavaScript.

## Getting Started

To get started, clone this repository and run the following commands:

```bash
npm install
```
This will install the necessary dependencies for the project.

## Development

It is recommended to use the VSCode Live Server extension to run the project
locally. This will allow you to see changes in real-time as you make them. There
is no need to run a build process or refresh the page manually. Additionally,
you do not need to setup a local server to run the project.

## Testing

To run the tests for the project, run the following command:

```bash
npm test
```

## Accessibility Lab Answers
Color:
The text is difficult to read because of the current color scheme. Can you do a test of the current color contrast (text/background), report the results of the test, and then fix it by changing the assigned colors? The lighthouse test reports "Background and foreground colors do not have a sufficient contrast ratio." before making any changes. It appears to flag ~37 elements. The lighthouse accessibility total score is 85. 
After fixing the lighthouse recommended changes under Contrast, the score increases to 89.

Semantic HTML:
The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.
Can you update the article text to make it easier for screen reader users to navigate?
The navigation menu part of the site (wrapped in <div class="nav"></div>) could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update.
Note: You'll need to update the CSS rule selectors that style the tags to their proper equivalents for the semantic headings. Once you add paragraph elements, you'll notice the styling looks better.