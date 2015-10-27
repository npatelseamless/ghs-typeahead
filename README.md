# ghs-typeahead - [AngularJS](http://angularjs.org/) directives specific to [Bootstrap](http://getbootstrap.com)

***
## Why this is forked?

Bootstrap's Typeahead didn't fit our needs and purposes so we extended it so that it could:

1. Display the dropdown simply by clicking on the input box (Very useful if you want to display data that is already cached)
2. Allow a ngDisabled field that made the row unclickable (Sometimes you want to show results for transparency reason)
3. Allowed refreshing of the rendered dropdown without closing and opening it.

## Demo
Pull down the latest code and generate the demo html file to play with the typeahead
```
git clone git@github.com:grubhub-umami/ghs-typeahead.git
cd ghs-typeahead
grunt watch
```
Open up the dist/index.html in the browser of your choice

## See It In Action
- Clicking on input box displays autocomplete popup (useful for showing cached data like the "Saved Addresses")
- ngDisabled shows the element as not clickable in the row
- Allow refreshing of the dropdown without closing & opening
![alt text](https://github.com/grubhub-umami/ghs-typeahead/raw/master/misc/images/focus-popup.gif "Focus Popup Autocomplete Visible")

## How to Use
The prerequesite for ghs-typeahead is to have angular-bootstrap.  Unfortunately at this time it still has a dependency on ui.bootstrap.position.  The easiest way is to use bower to install it.  I have not published this to bower so you'll unfortunately have to install the repository directly instead
```
bower install https://github.com/grubhub-umami/ghs-typeahead.git#<TAG_VERSION>
```
Please note that the <TAG_VERSION> should be replaced with the version number that you are interested in.  Add the ghs.bootstrap.typeahead module to your application and you should be able to use the typeahead directive as expected.

## How to Develop
If you wish to fork the project please feel free.  To generate a sample of your code run `grunt watch` and open dist/index.html in a browser of your choice.
To run the tests simply run `grunt test`
If you want to contribute please submit a PR.

