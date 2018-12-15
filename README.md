# Burrow
A client/browser that accesses _gopherspace_. It is under current early stage development.

 ![Burrow browser](http://brianmevans.com/files/burrow_01.png "Burrow v0.1.8 main window")

## Gopher
[_Gopher_](https://en.wikipedia.org/wiki/Gopher_(protocol)) is a communications protocol that, in the early 90s, competed (briefly) with what became the world wide web. _Gopher_ serves up files and text based menus. As such, it is much lighter weight than HTML documents and the like served over http. Due to its text based nature it also has the benefit of being reliable in its visual output and style, and for being relatively accessible. 

## Browser Features
The following is a list of current and future Burrow features:

- Tk based GUI
    - Back button, move backwards in session history
    - Forward button, move forward in session history
    - Ffavorite button adds current page to favorites __(non-functional)__
    - Home, shows favorites and is a start page
    - An address bar, on _ENTER_ submits a request for a _gopher_ page
    - Settings button, brings up configuration menu __(non-functional)__
    - A display area for the requested information
    - Scroll bar
    - A status bar to display various information
- Links
    - On hover, link destination shows in status bar
    - On hover, link is underlined
    - Links are colored differently from regular text _(configurable)_
    - Link type appears next to link in noticeable coloring _(configurable)_
    - On primary click, destination is loaded and new location replaces old location in address bar
    - On primary click, link background changes to visually confirm click _(configurable)_
    - Cursor is a pointer over links, while regular text is an I-beam cursor.
- Menus, Pages, and Files
    - Menus display clickable links
    - Text files display in the viewport
    - Image files display in the viewport
    - Right click on image allows for download __(non-functional)__
    - Sound files __(non-functional)__
    - Binary files __(non-functional)__
    - HTML files, open in a new tab in the default web browser
    - Interactive pages/search __(non-functional)__
- History
    - Session based history for backward and forward navigation
    - Persistent favorites __(non-functional)__
    - Suggestions on URL entry based on persistent history __(non-functional)__
- Application settings and menus
    - Settings menu __(non-functional)__
        - Color themes
        - Icon themes
        - History settings
        - Files/download settings
    - Secondary click context menus for text manipulation & file saving __(non-functional)__
    - Page saving for offline viewing __(non-functional)__
    - Hotkey to view page source for menus __(non-functional)__
- Errors
    - Error warnings to user __(non-functional)__
    - Error page on bad/malformed request __(non-functional)__
    - Error display for type 3 server response __(non-functional)__


## Installation

Burrow requires python3 to be installed on the system prior to running.
Until some bundling/setup-file creation occurs, you will also need to add:
    
    pip3 install pillow
    

On some linux distributions an additional package for tkinter may be required.
If you get a console error complaining about tkinter try the following (or equivalent for your package manager):

    sudo apt-get install python3-tk
    sudo apt-get install python3-pil.imagetk
    

## Distribution

Burrow's primary system target is debian based linux systems. Once a version 1.0 is reached the plan is to distribute via .DEB packages and possibly through snapcraft (if a workable bundle can be figured out).

Some version of windows executable may come along as well, depending on configurability of build tools (py2exe, freeze, etc) for windows executables and time.


## Contribute

To contribute, please branch off of `develop` and then submit a pull request into `develop` with any changes. As the project grows I will likely add wiki, issues, etc as the need arises and more people get involved.


## Disambiguity

There is [another project](https://github.com/jamestomasino/burrow) by the name of Burrow (that predates this one) by _jamestomasino_. It is a really cool collection of tools for managing gopher sites/projects. I definitely recommend checking it out!
