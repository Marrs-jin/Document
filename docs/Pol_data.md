## Subdirectories for data used
All data folders need to be in the same directory as the codes are. The folders at this level are:
<ul>
<li>TXT Files</li>
<li>CSV Files</li>
<li>HTML Files</li>
<li>Python Scripts</li>
<li>Zip Files</li>
</ul>

**TXT Files** have all the data that are used to create the graphs.  

**CSV Files** Create the CSV format of these txt files as in the CSV Files folder. These files will be passed to the Python script as the input files.

**Python Scripts** has the scripts used in generating the polarizability pages. Provide the name of the generated .csv files in the related python scripts that have been provided in the Python Scripts folder. As a result you can see the generated graphs created in html format. Bokeh library is used for creating these graphs.

**HTML Files** have the final HTML files of all the grpahs and the main polarizability webpage that loads the requested graph to the page. The main polarizability webpage loads the related graph html file into the iframe section of the page based on the button selected by the user.

**Zip Files** are the text files that would be downloaded when the user clicks on Download Data Button. For combined graphs you need to zip all the data files related to that graph.

When all the graphs are created make the required changes to the main NaPolarizability.html webpage so that correct HTML files are loaded to the iframe section of the page with each click of the button.
