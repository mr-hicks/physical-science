# A lesson plan blog

This website is generated by Github using Jekyll (a static website generator) and hosted on Github Pages.

The main sections/features are:

  * The front page has the student blog which allows students to access the materials they require as well as letting them know what we are doing.
  * There is a student resource section
    *  Useful link repository
    *  Archive of the current year
  * There is an educator resource section that has:
    * Collection of units/info taught
        *   Generated based off of the readme files for each unit - the first paragraph
    * The notes/comments from how each lesson went
        *   When a given unit is clicked on, the pages tagged with edu AND unit are displayed.
    * Sortable either by lesson or date/year
    * Host to personal notes of how to setup things, like a personal blog
    * Links relevent to teachers.
  * About page discusing what the page is and its purpose

## Tags
Each page should be tagged for sorting, either by tag or in the yaml front matter on each page.

  * Unit tag - for sorting into units later
  * stu vs edu (stored in the jekyll front matter yaml)

## Scripts
### Student -> Teacher
It is becoming apparent that I should have seperate teacher/student blog pages.
The idea is, at the end of the day I can run a script on the student page which copies the file and contents, appends _edu to the name, and changes the yaml page type from stu to edu

### Versions...
This is not very important but should be noted, the blog will always point at the current lesson EVEN if it is an old entry.
It would be nice if there was an easy way to access the blog on the git version that uploaded at that time...

## Change log
For trial/practice/understanding I'm re-doing the process I previously did to manipulate the default minima blog into what I want.
Note that changes to _config.yml require a restart of the blog to take hold.

  * jekyll new --force . {specify the directory as local}
  * Add the _includes, _layouts, _sass, assests folders so I can modify things.
  * Copy from the minima source into the layouts to modify the layouts
  * Add header_pages: to the _config.yml file to specify the headers.
  * Add and modify the date settings to match my prefered day-name day mon year

## Needs
  * Tag based edu page - generated from the first paragraph of the units readme files
  * unit pages generated based on the readme file + all posts with the respective unit tag and edu
  * sort the pages that appear on the font to be stu pages, ordered by date.
  * a way to refer to the unit readmes dispite their being an additional layer down.
  * then modify the default pages to have the convient navigational features added in the lynda.com tutorial.