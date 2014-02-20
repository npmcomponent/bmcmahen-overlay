*This repository is a mirror of the [component](http://component.io) module [bmcmahen/overlay](http://github.com/bmcmahen/overlay). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/bmcmahen-overlay`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# Overlay

  Super simple overlay.

## Installation

```
$ component install bmcmahen/overlay
```

## API

### overlay()

  Returns a new `Overlay`.

### Overlay#show()

  Show the overlay.

### Overlay#hide()

  Hide the overlay.


## Events

  - `show` when the overlay is showing
  - 'shown' when the overlay is shown
  - `hide` when the overlay is hiding
  - `hidden` when the overlay is hidden (removed)

## Example
```
var Overlay = require('overlay');
var overlay = Overlay.show();
setTimeout(function(){
  overlay.hide();
}, 5000);

overlay.on('hidden', function(){
  // overlay is fully hidden
});
```

## License

  MIT