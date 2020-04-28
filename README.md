This README file contains the steps taken to create a website. 
1.	New Repo:	
	⁃	Use the CI template to create a new workspace / repo 
2.	Gitpod: setting up new workspace:
	⁃	create assets folder with subdirectories: images and css
	⁃	within the css folder >> style.css
	⁃	create index.html file (standard homepage)
3.	Setting up index.html 
	⁃	put in basic HTML boilerplate code (!DOC etc)
	⁃	change the title to project name 
	⁃	add external links to CDNs that will be used (Bootstrap, FontAwesome, Google fonts etc)
	⁃	add link to stylesheet 
	⁃	create a test to see whether code is linked properly to css etc
4.	Structuring your doc 
	⁃	add header, section, footer tags
	⁃	add comments about what content will go in these sections 
	⁃	save file, use git add command to add files to the git repository 
	⁃	use git commit command with “Initial commit” for first commit 
	⁃	test again to make sure project runs and that the server is running in the browser 
5.  Setting up the grid layout 
    -   if using Rule of Thirds: splitting the screen into 3rds >> set up row and column classes.. if using Bootstrap i.e.
        - div class="row"
        - div class= "col-md-4" (1/3)
        - div class= "col-md-8" (2/3)
        - note: in Bootstrap the rule is that the direct child of the row class must be a column class 
        - when you create a class="col" without a number it creates a full width bootstrap column 
6.  Next step = setting up your fonts and linking them in the stylesheet (you can either link it in the head or import it
        using the import syntax in Google Fonts and then adding the font weights) >> i.e. link...Roboto:100,200,300'); etc
7.  Set up the page 
        - set up margins 
        - set up header >> if you have a logo its standard practice that logo should be a link which links back to homepage
        - when setting up font-family make sure to include a fallback font in case your chosen one doesnt load ie 
            = font-family: "Exo", sans-serif 
        - also include comments in your stylesheet to mark different style sections 

NOTE:
***The other thing that we have to do is a little CSS hack.***
1. When we display items inline, then the white space that's in our HTML file becomes visible as a single space between our items.
    - The way to solve this is to create a container with the font-size of 0 so that the spaces are not displayed.
    - So we're going to add the menucontainer class to our <ul>.
    - Then in our CSS, we'll target it here, and we'll give that a font-size of 0, which will close up the gaps between our items.
    - The problem is that means that all of our items will then have a font-size of 0, so we can no longer see them.
    - We can override this by using our nav ID, targeting all the children lis and giving a font-size of 14px.
    - We'll then also just set the padding to 0 as well because we want to have full control over that.
    - So the gap has closed up, but it's still not quite right.
    - We've got this opening gap here now that we need to close.
    - The reason for this is that Bootstrap actually provides padding to all the columns by default.
    - This is called a gutter so that there's a space before and after the columns.
    - To fix it, we can add the no-gutters class to all of our rows, and this will switch off the gutters for the columns.
2. when adding font-awesome icon , use the <i> and class="fa" for font-awesome followed by the icon class name 
    - by using aria-hidden="true" >> it is ignored by screen readers 
