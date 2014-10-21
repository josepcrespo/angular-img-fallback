AngularJS Image Fallback Module
===============================

AngularJS Module to manage the fallback of the `src` attribute of the `img` HTML element. It has `fallback-src` to handle erros in image loading and `loading-src` for images loading placeholders.

## Bower Download
`bower install angular-img-fallback-directive --save`
  
## Installation
1. Add a similar line (depending on your paths) to you HTML to import the script into your page.<br />
`<script src="lib/angular-img-fallback/angular-img-fallback.js"></script>`
2. Add `imgFallback` to your angular app module dependencies list.<br />
`angular.module('myAngularApp', ['imgFallback']);`
3. Add the `fallback-src` attribute to your img<br />
`<img ng-src="path/to/img.jpg" fallback-src />`


## Usage
Just add the `fallback-src` and the `loading-src` attributes to your `<img />` tags<br />
`<img ng-src="path/to/img.jpg" fallback-src loading-src />`<br />
Make sure you use `ng-src` as your image src attribute.


## Advanced options
- Simple usage, will replace to a default missing image placeholder<br />
`<img ng-src="path/to/img.jpg" fallback-src />`

- Custom fallback, will replace to your own custom missing image<br />
`<img ng-src="path/to/img.jpg" fallback-src="path/to/fallback.jpg" />`

- Loading placeholder, show a loading placeholder until image loads<br />
`<img ng-src="path/to/img.jpg" loading-src="path/to/fallback.jpg" />`

- Custom Loading placeholder, show a custom image loading placeholder until image loads<br />
`<img ng-src="path/to/img.jpg" loading-src="path/to/loading.jpg" />`


## Icons license
Icons are provided from http://icomoon.io/ under the GNU General Public License v3.0<br />
http://www.gnu.org/licenses/gpl.html
