### v1.5.12

* Fixed: parse single and double quotes.
  
### v1.5.11

* Fixed: New `enableScssFindUsage` setting was mis-behaving. Now it is fixed.
  
### v1.5.10

* Fixed: Slow intellisense due to SCSS usage indexing. Disabled by default try this to enable:

```
  "html-css-class-completion.enableScssFindUsage": true,
```
  
### v1.5.9

* Fixed: Multiline ids are not processed due to wrong variable executed in second.
  
### v1.5.8

* Fixed: Do not show same file twice.

### v1.5.7

* Added: ID completions by pressing `#`

### v1.5.6

* Fixed: Multiple occurrences...
  
### v1.5.5

* Added: PHP parser
* Added: Separate ID and Class completion.

### v1.5.4

* Fixed: PHP and SCSS find usages
* Fixed: No new line on found usages (descriptions)

### v1.5.3

* Fixed: Incremental build contains deleted items
* Incremental build is seems to be stable. With this build, We also remove unused definitions from autocomplete.

### v1.5.2

* Fixed: Find usage issue

### v1.5.1

* Fixed: Find usage issue

### v1.5.0

* Added: Find usage locations in scss/css files. **WIP**

**Still on-going. Do not use it on production.**

### v1.4.0

* Incremental changes. We are only update changed parts. This saves lot of CPU and time. Your workspace will be scanned once you open VSCode, after that everything will be incremental. (**BETA**)

Let me know if anything goes wrong for you by opening an issue on GitHub...

### v1.3.1

* Fixed #14:
  + Prevent re-cache everytime.
  
### v1.3.0

* Fixed #4, #5, #7, #8, #9, #10, #11: 
  + Better ID tag parsing.
  + Ability to show suggestions from HTML to CSS/SCSS
  + Latte template support. (Both directions)
  + Fixed .vue class autocompletion issue
  + exclude node_modules/ from cache. This causes high cpu load.
  + pressing " or ' will trigger autocomplete. No need for space anymore.
  
### v1.2.1

* Fixed #6. Extension autocompletes weird "class" strings in html, js and css.

### v1.2.0
* Ability to show suggestions from HTML and Slim templates in CSS/SCSS.
  
  You can define class names in HTML and Slim templates and see their results in CSS/SCSS. (vice-versa).
  Note: If you **save** any html or slim template, cache will be reinitialized. I am thinking to do the same for CSS/SCSS.

### v1.1.0

* Added SCSS/SASS support without compiling whole package.
* Ability to parse custom and magic functions
* Ability to get remote css files such as bootstrap. Remote CSS files will appended to temp dir of your OS.
* Fixed localFiles variable stay in if.
