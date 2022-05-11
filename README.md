# Accessibility improvements and style sheet consolidation


## Aims of the project
1. Improve the accessibility of the webpage through utilization of semantic HTML elements and appropriate alt descriptions for certain images
2. Consolidate the CSS style sheet by eliminating duplicate code
3. Organize both the index.html file and the style.css file according to the visual flow of the webpage and for better readability for future developers

</br>
### 1. Improve the accessibility of the webpage through utilization of semantic HTML elements and appropriate alt descriptions for certain images
The original index.html file code had many `<div>` elements where a more specfific HTML semantic element could make the webpage more accessible and readable. 

For example, the header element was written as `<div class="header">` rather than `<header>`; so I changed it to `<header>` and made the corresponding change in the CSS style sheet (".header" to "header"). 

Additionally, I created sections for the services and the benefits and within those sections used `<article>` elements instead of `<div>` eleements for greater accessiblity and clearer organization.

For images whose presence enhanced the information being presented, I added concise alt descriptions. This along with the afore-mentioned changes to HTML semantic elements works to better serve webpage visitors who utilize screen reading technology.


### 2. Consolidate the CSS style sheet by eliminating duplicate code
In the CSS style sheet, there were many instances of duplicate code for each article in the sections, which I consolidated by better utilizing the "class" attribute. 

For example, in the "services" `<section>`, each `<article>` was given it's own class with corresponding styles in the style sheet. However, many of these styles repeated for each `<article>`, and so I consolidated those styles into one class and assigned that one class to each article, greatly consolidating the code in the style sheet.

This helps future developers when they go to work on the style sheet in the future so that they aren't having to scour the sheet for each instance of duplicate code to change it.


### 3. Organize both the index.html file and the style.css file according to the visual flow of the webpage and for better readability for future developers
Both the index.html and style.css files lacked comments and spacing that helped show the organizational flow of the code, and so I added spacing and comments to set off each section to make the documents easier to read.

For example, in the index.html file, I separated the "services" `<section>` and the "benefits" `<section>` and used the comments "services section" and "benefits section" (respetively) at the start of each section.

In the style.css file, many of the attributes were out of order from how the appeared in the index.html file, and so I rearranged the attributes to correspond with the order in which their respective elements appear in the index.html file. 

For example, the "service" attributes were placed below the "benefits" attributes on the style.css file, though the "service" articles code is before the "benefit" articles code on the index.html file. Thus, I moved the "service" code in the style sheet to be above the "benefit" code.

Additionally, I used comments to label each section of styles in the style sheet. For example, above the first line of code for the "footer" styles, I added a comment that says "footer styles start" and below the last line of code for the "footer" styles, I added a comment that says "footer styles end" so that it is easy to see where each section's styles begin and end. Such comments can help future developers easily find where to go to work on a particular section's styles.
