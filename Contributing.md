#   Contributing to the Project

##  Tools Used

-	IntelliJ Community Edition
-	Markdown
-	Mermaid
-	YAML

##  Adding New Pages

Adding new pages to the documentation is a straightforward process. Each page should be created as a Markdown file (.md) and placed in the appropriate directory based on its content.

All pages should have a YAML header section with the following minimum information:

    ---
    title: Homepage
    description: "Homepage for Yet Another Architecture Framework"
    ---

Whenever pages are added to any directory update the index.md file in that folder to include the new page to the list of children. 
For example, if you add a new page called "NewPage.md" to the Blogs folder, you would update Blogs/index.md to include NewPage in the children list as follows:

    ---
    title: Blogs 
    children : 
        -   EnumeratedValues
        -   ImportanceOfNames
        -   NewPage
    ---

The index.md file replaces what would normally be the ReadMe file for that folder and serves as the landing page for that section of the documentation.
This should include a brief description of the content of that section and Markdown links to the individual pages within it.

For example, the Blogs/index.md file might look like this:

    ---
    title: Blogs 
    children : 
        -   EnumeratedValues
        -   ImportanceOfNames
        -   NewPage
    ---
    
    ...some introductory text about the content of the Blogs section...

    - [Enumerated Values](./EnumeratedValues.md)
    - [Importance of Names](./ImportanceOfNames.md)
    - [Importance of Names](./ImportanceOfNames.md)

Every should have a "Back" link to its parent index.md file and every index.md file should have a "Home" link to the root index.md file. 
This allows for easy navigation through the documentation.