# fis-parser-ejs

a parser plugin for fis to compile ejs file

## usage

1. install

    ```bash
    npm install -g fis-parser-ejs
    ```

1. configure

    ```javascript
    //tell fis that `.ejs` is a js file
    fis.config.set('roadmap.ext.ejs', 'js');
    //tell fis that parse `.ejs` file by using `fis-parser-ejs` plugin
    fis.config.set('modules.parser.ejs', 'ejs');
    //set options if you need
    //@see https://github.com/visionmedia/ejs#options
    fis.config.set('settings.parser.ejs', {
        open : '<#',
        close : '#>'
    });
    ```