# XLIFF to JSON converter
## This script grabs all ```<source></source>``` and ```<target></target>``` content and generates JSON with it.

## Sample input
```
<?xml version="1.0" ?>
<xliff version="1.0">
    <file original="global" source-language="en_US" target="fi" datatype="plaintext">
        <body>
            <trans-unit id="1">
                <source>header.home</source>
                <target>Homepage</target>
            </trans-unit>
            <trans-unit id="2">
                <source>header.authors</source>
                <target>Authors</target>
            </trans-unit>
            <trans-unit id="3">
                <source>header.more</source>
                <target>More</target>
            </trans-unit>
        </body>
    </file>
</xliff>
```

## Output
```[{"source":"header.home","target":"Homepage"},{"source":"header.authors","target":"Authors"},{"source":"header.more","target":"More"}]```

**Node.js is required to install and run this script**
## Installation && usage
1. Run in your terminal ```npm i xliff_to_json_converter``` to install this script locally.
2. Start conversion (from your project root folder) by:  
```node ./node_modules/xliff_to_json_converter/bin/run.js <yourExistingTranslationFile.xliff> <outputFileToCreate.json>```
3. Have fun!

## Global installation && usage
1. Install this script globally by typing: ```npm i -g xliff_to_json_converter```
2. Run it from every folder like this:  
```xliff_convert <yourExistingTranslationFile.xliff> <outputFileToCreate.json>```
3. Have global fun!

## License
### **MIT**
**Copyright 2017 Marcin Kołodziejczak**

>Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
>The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.