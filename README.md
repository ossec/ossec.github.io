# ossec.github.io

These are the files for the official OSSEC Project website. They are built automatically 
from the ossec/ossec-docs repo by Travis when pull requests are made for that repo 
after the website source files are updated.

## Requirements

The main website files consist of Sphinx and HTML template files, so you require 
the Python and sphinx-build to update the website. In most cases you will need to 
modify the website when a new OSSEC release has been created or a blog entry is 
added.

## Updating the Downloads page

1. Fork the ossec/ossec-docs repo
2. cd into the ossec-docs directory
3. Edit the downloads.rst file
4. Run *make html*.
5. Open the _build/html/index.html file in a browser.
6. Check to see the test wbesite looks OK.
7. Repeat steps 3-6 until you have it the way you want.
8. Push you changes to your fork of ossec-docs.
9. Create a pull request for your changes.

## Adding a blog entry

1. Fork the ossec/ossec-docs repo
2. cd into the ossec-docs directory
3. Add your blog entry to the blog/posts directory. The naming convention is *YYYY-MM-DD-title.rst*.
4. Add the following code to your blank file: 
<pre>
.. post:: MMM DD, YYYY
   :tags: 'your tags'
   :category: 'your categories'
   :author: 'your name'
<pre>
5. Put your date, tags, categories, and name in the corresponding fields.
6. Add a title below this section that has a row of '=' before and after the title that are the same charter length as the title.
7. Add and edit your content below the title.
8. When you are done writing, run *make html*.
9. Open the _build/html/index.html file in a browser.
10. Check to see the test wbesite looks OK.
11. Repeat steps 7-10 until you have it the way you want.
12. Push your changes to your fork of ossec-docs.
13. Create a pull request for your changes.

 



