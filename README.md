HTML Structure:

<!DOCTYPE html>: Declares the document type and version of HTML being used. It ensures that the browser renders the page in standards mode.
<html lang="en">: Defines the root element of the HTML document and specifies the language as English for screen readers and search engines.
<head>: Contains metadata about the HTML document, such as the character set and title.
<body>: Contains the visible content of the HTML document, including the header, main content, and JavaScript code.

  Header Section:
  
<div class="header">: Defines a section at the top of the page for the header content.
<a href="https://your-main-website.com" class="home-link" onclick="returnToHome()">Home</a>: Creates a link labeled "Home" that points to a main website. The returnToHome() function is called when this link is clicked, but the function is not defined in the provided code.
<h1>PROJECT MEDIAWIKI</h1>: Displays the title "PROJECT MEDIAWIKI" at the center of the header.
Font controls: Provides controls for adjusting font color and size.

  Search Bar:
<div class="search-bar">: Defines a section for the search bar.
<input type="text" id="searchInput" class="form-control" placeholder="Search Wikipedia">: Creates a text input field where users can enter their search queries. The placeholder text inside the input field suggests to users what they can search for.
<button class="btn" id="searchBtn" type="button" aria-label="Search Wikipedia">Search</button>: Creates a button labeled "Search" that users can click to initiate a search.
Main Content Section:
<div class="main-content" id="results">: Defines a section for displaying search results. The id="results" attribute is used to target this element in JavaScript for dynamically updating its content.

  JavaScript:
searchWikipedia(): Defines a function that fetches Wikipedia search results based on the user's input. It constructs a URL with the search term and fetches data from the Wikipedia API using fetch().
displayResults(data): Defines a function that displays the retrieved search results on the webpage. It extracts relevant information from the API response and dynamically generates HTML elements to display each search result.
Event listeners: Attach event listeners to the search button, search input field (listening for Enter key press), and font size input field. These listeners trigger specific actions when events occur, such as initiating a search or adjusting font size.
toggleColorPicker(): Toggles the display of the color picker for font color selection.
changeFontColor(): Changes the font color of search results based on the selected color from the color picker.

Styling:
Custom CSS styles are applied to create a layout resembling Wikipedia. Styles include background images, font styles, layout alignments, and button appearances.
The Teko font from Google Fonts is imported and applied to the entire document.
Bootstrap is included to enhance styling consistency and provide additional design elements.

API Integration:
The Wikipedia API is used to fetch search results based on user input. The fetched data is then processed and displayed on the webpage.
This breakdown explains each component of the provided code in detail, including its purpose and functionality.
