*This repository is a mirror of the [component](http://component.io) module [tomerdmnt/tag-input](http://github.com/tomerdmnt/tag-input). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/tomerdmnt-tag-input`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# tag-input

  A [component](http://github.com/component/component) that turns a text input element into a pretty tags input.
  Enables you to work with any MVC framework using simple events or you can get the tags from the inner model.

  ![Tags Input](https://raw.github.com/tomerdmnt/tag-input/master/screenshot.jpg)

## Install
  ```
    component install tomerdmnt/tag-input
  ```

## Example

  ``` javascript
    var TagInput = require('tag-input');

    var taginput = TagInput(document.getElementById('tags'))

    taginput.on('add', function (tag) {
      console.log(tag + ' added')
      console.log(taginput.tags())
    })

    taginput.on('remove', function (tag) {
      console.log(tag + ' removed')
      console.log(taginput.tags())
    })

  ```

## Notes about style
  The pseudo input style is very basic, so you can adjust its looks to your site, You can extend it by adding to taginputContainer class.

## api

### TagInput(input)
  binds to a text input element

### addtag(tag)
  adds a tag to the tag input from js

### removetag(tag)
  removes a tag from the tag input from js

### event: 'add'
  Called when a tag is added

### event: 'removed'
  Called when a tag is removed`


