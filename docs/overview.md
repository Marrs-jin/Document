# Description of the site
The web portal is composed of a collection of static HTML pages (pages ending in the .html file extension). Each page is separated into a few different components:

<ul>
<li> Imported libraries
<li> CSS stylings
<li> JavaScript or jQuery functions
<li> HTML elements and the tabular data
</ul>

## Imported Libraries
At the top of every file there is a series of read in statements. These are the libraries that are being read in for functionality of the site.
Listed below are some, but not all (as this is unique to the type of page), of the functionalities that might be read in by these commands.

### &bull;Default stylings
Default stylings for the page or an element of the page. These lines often start "<link rel="stylesheet"...".
These pull, often from bootstrap (an open source CSS framework), stylings for the different parts of the page. Examples would be the default color
of buttons or the size of containers. These defaults can be manually changed, see the "CSS Stylings" section.

### &bull;Functions
Functions controlling how the page reacts. These lines often start "<script src =...". These lines are needed to control how the
DataTables objects let users download excel data, how the modal objects control the pop-ups when users click on "Help" or "info", or how
the Google Analytics section works (this is the function written at the top of the import section). See the "Google Analytics" section for more information.

### &bull; Miscellaneous
If a page uses images or custom functions they are loaded in here as well. This includes the "ASD" logo and the customized way the info button clicks are handled.

## CSS Stylings
Below the library read-ins is where manually created settings are written. Code that is written in-between `**<style> </style>**`
blocks are "CSS" stylings. This code controls the visual aspects of the page. These styles are written above the data tables.
If a user wished to change some funadmental style of the page,
such as changing the button's size or the header's text color, they should first see if these are being declared in the written CSS sections.
If that style is not explicitly written in the page, then the style must be being handled with the libraries being read in.

## JavaScript or jQuery Functions
There are several unique functions in the web pages that had to be written specifically for some use in that page. These include
how the data is sorted when a user clicks on a state button, how the excel download works (filename, data type, which table to download),
and making the "Print" and "Excel" buttons visible on a state button click.

These functions are located in-between `**<script> </script>**`
blocks, either at the top of the page above the data tables or the bottom of the page below them.
If a user wishes to change how some function is handling events they should first check if that function was manually written in the page.
If the function is not explicitly written in the page, then the function must be being handled with the scripts being read in.

## HTML elements
The rest of the code is the HTML. This is generally what the user will see when they open the web page. Exceptions are hidden elements, such as the excel data table.
Items in this class include all buttons, all tables, and all visible text on the page.
