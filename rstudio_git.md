Using Git with RStudio
================
Andrew Ruether
July 5, 2022

# Overview of git and GitHub

## Why Software Version Control?

-   Backup
-   Deploy on multiple computers - work from anywhere
-   Keep track of changes - revert if needed
-   Freeing (do you have large, commented out sections or multiple
    versons of the same file?)
-   Collaboration
-   Fancier use cases
    -   Run automated tests
    -   Deploy automatically to production server
    -   Keep track of issues

## Git versus GitHub

-   git - open source software version control program
    -   Used to keep track of changes to software, allow multiple people
        to work on the same code, deal with conflicts
    -   Most widely used
    -   Command line
-   GitHub - company formed to create services around git
    -   GitHub.com
    -   GitHub Enterprise (github.swarthmore.edu)
    -   Nice website
    -   Issues, wikis, collaboration tool, web publishing
    -   Most widely used (alternative - GitLab)

# Getting Started with Git

## TIMTOWTDI

-   Use RStudio’s git controls
-   Use git from the command line
-   Use another git client

## New Repo

-   Log into github.com and create a new repository (project)
    -   Public
    -   Add a README
    -   .gitignore ==\> Select R
    -   License: <https://choosealicense.com>

## Make some changes

-   Click on the pencil icon to the right of the README.md file
-   Make some edits in markdown format
-   Commit changes
-   Repeat
-   View commits log

## Connect RStudio to GitHub

-   Create a new GitHub authentication token
    -   Settings → Developer Settings → Personal Access Tokens
    -   User, repo, gist, workflow permissions
-   Save token somewhere safe (e.g. LastPass)  
-   In RStudio: gitcreds::gitcreds_set()

## Create new RStudio Version Control Project

-   New Project → Version Control → Git
-   Paste in Repo url (HTTPS)
-   Make changes
-   Git pane
    -   Commit changes
    -   Push to remote

## Publishing

-   GitHub can render .md files → `output: github_document`
-   Can use GitHub Pages to render HTML output
    -   Repo settings → Pages

# Additional info

## References

-   RStudio Version Control:
    <https://support.rstudio.com/hc/en-us/articles/200532077>
-   GitHub and RStudio:
    <https://resources.github.com/github-and-rstudio/>
-   Happy Git and GitHub for the useR: <https://happygitwithr.com/>
