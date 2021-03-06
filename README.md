# Tutorial server

Hi everyone!

This is a standalone server for the javascript tutorial https://javascript.info.

You can use it to run the tutorial locally and translate it into your language.

# Installation

If you have an old copy of the English tutorial, please rename `1-js/05-data-types/09-destructuring-assignment/1-destructuring-assignment` to `1-js/05-data-types/09-destructuring-assignment/1-destruct-user`.


1. Install [Git](https://git-scm.com/downloads) and [Node.JS](https://nodejs.org).

    These are required to update and run the project.
    For non-Windows OS use standard install tools (packages or whatever convenient).
    
    (Maybe later, optional) If you're going to change images, please install [GraphicsMagick](http://www.graphicsmagick.org/).

2. Install global Node modules:

    ```
    npm install -g bunyan gulp
    ```

3. Create the root folder.

    Create a folder `/js` for the project. You can use any other directory as well, just adjust the paths below.

4. Clone the tutorial server into it:

    ```
    cd /js
    git clone https://github.com/iliakan/javascript-tutorial-server
    ```

5. Clone the tutorial text into it.

    The text repository has `-language` at the end, e.g `ru`:
    ```
    cd /js
    git clone https://github.com/iliakan/javascript-tutorial-ru
    ```

6. Run the site

    Run the site with the language:
    ```
    cd /js/javascript-tutorial-server
    ./edit ru
    ```

    Please note that the argument of `edit` is exactly the language you cloned at step 5.
    
    Wait a bit as it reads the tutorial from disk and builds static assets.

    Then access the site at `http://127.0.0.1:3000`.

7. Edit the tutorial

    As you edit text files in the tutorial text repository (cloned at step 5), 
    the webpage gets reloaded automatically. 
    
    
# TroubleShooting

If something doesn't work – [file an issue](https://github.com/iliakan/javascript-tutorial-server/issues/new).

--  
Yours,  
Ilya Kantor 