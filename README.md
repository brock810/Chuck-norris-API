# Chuck-norris-API
The code is an HTML page showing Chuck Norris jokes. It has a button to fetch jokes, options to share/copy/like them, and an expandable sidebar with Chuck Norris facts. It's visually appealing with animations. JavaScript handles fetching jokes and user interactions.
HTML Structure:

The HTML structure defines the layout and elements of the web page. Here are the key elements in the code:
<head> Contains the metadata and external resources used in the page, such as the title, stylesheets, and scripts.
<body>: Represents the main content of the page.

  CSS Styling:  
The CSS code defines the styles and layout for various elements in the page. It is used to control the appearance and animations. Here are the main CSS styles used:
body: Sets the background image, font family, text color, and other properties.
h1: Styles the title of the page, including the font size, color, and animation.
#joke: Styles the joke text, including the font size, color, and text shadow.
#get-joke-button: Styles the "Get Joke" button, including the background color, text color, and hover effect.
.loading: Styles the loading text that appears when fetching a joke.
.share-button: Styles the share button, including the background color and hover effect.
.like-button: Styles the like button, including the background color and hover effect.
.sidebar: Styles the sidebar that displays Chuck Norris facts, including its width, background color, and font color.
.fact: Styles each individual fact in the sidebar, including the font size and color.
.image: Styles the images in the container, including the width, height, and border radius.

JavaScript Functionality:
The JavaScript code provides the functionality for the Chuck Norris Jokes application. Here are the key JavaScript functions and their purposes:
getRandomBackground(): Returns a random background image URL from the backgrounds array.
changeBackground(): Changes the background image of the page by updating the CSS background-image property.
showLoading(): Shows the loading spinner and disables the "Get Joke" button.
hideLoading(): Hides the loading spinner and enables the "Get Joke" button.
shareJoke(): Opens a new window with a Twitter intent to share the current joke.
copyJoke(): Copies the current joke to the user's clipboard.
setLocalizedText(): Sets the text content of various elements on the page based on the selected language.
switchLanguage(lang): Switches the language of the page based on the user's selection.
likeJoke(): Displays an alert when the "Like Joke" button is clicked.
initializePage(): Initializes the page by setting the localized text, changing the background, fetching a joke, and displaying a message after a certain delay.
Event Listeners:

The code includes event listeners that trigger specific actions when certain elements are interacted with:
DOMContentLoaded event: Fires when the initial HTML document has been completely loaded and parsed.
click event on the "Get Joke" button: Calls the fetchJoke() and changeBackground() functions.
click event on the "Share Joke" button: Calls the shareJoke() function.
click event on the "Copy Joke" button: Calls the copyJoke() function.
click event on the "Like Joke" button: Calls the likeJoke() function.
click event on the sidebar facts: Toggles the visibility of the clicked fact.
