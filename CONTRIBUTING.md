"Have you found a bug ?" or "Do you want to contribute in making 'natural-cron.js' more flexible ?"<br/><br/>
We would definitely like to hear a big "yes" from you. Just make sure to follow the guidelines below, we are eager to see your contribution as a part of this library.
***

If you have new English phrases that don't work with `natural-cron.js` yet, please first discuss the change you wish to make via issue or email (darkeyedev@gmail.com) before making the changes.

## Guidelines:
* #### Before you begin...
    1) Make sure to check if there are any current open issues or pull requests regarding the same change that you want to make.
    2) Understand how the library works completely and feel free to reach us at darkeyedev@gmail.com for any confusion.
* #### Coding guidelines
    1) Follow the project directory structure.
    2) Keep the code well structured, simple & readable as much as possible.
    3) Follow proper naming conventions for variable & function names.
    4) Make sure to write comments wherever required (but not too much).
    5) Remove all debugging comments and log statements (if any) before final commit.
* #### Preparing final .js files
    1) We use `browserify` to bundle the JS code for browsers.<br/>
       Install [browserify](http://browserify.org/#install) with:
       > npm install -g browserify
       
       Go to `src` folder and run the following command:
       
       > browserify index.js -d --s getCronString > ../dist/natural-cron.js
       
       (This will prepare the `natural-cron.js` file and put it in `/dist` folder)
    2) We use `JSCompress` for minifying the bundled JS library.<br/>
       Head to [JSCompress](https://jscompress.com/) and generate minified JS code from `natural-cron.js` 
       file and put the minified code in `natural-cron.min.js` inside the same `/dist` folder.
* #### Testing guidelines
    1) If you have worked on some new English phrases, append those example phrases and their outputs in `/test/examples.js`
    2) Open `/test/autoTester.html` file in browser. It will automatically test all the examples in `/test/examples.js` file against specified desired outputs for both `/dist/natural-cron.js` & `/dist/natural-cron.min.js` files
    3) Test & verify that there are no wrong results in the above test & the updates implemented by you work as expected.
* #### and some final touches...
    1) Update `README.md` file accordingly (if required).
* ##### that's it, submit the pull request, feel proud and get relaxed :)
