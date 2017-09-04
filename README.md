MZO Image Comparison App
=================

<img src="icon.png" width="300">

The iPad App to compare two images, that accompanies the ['Majster z Okoličného a gotické umenie Spiša okolo roku 1500'](https://www.sng.sk/sk/vystavy/1064_majster-z-okolicneho-a-goticke-umenie-spisa-okolo-roku-1500) exhibition at the Slovak National Gallery, 7 September - 26 November 2017.
It is an open source mobile application built using Apache Cordova, written entirely in HTML, CSS and JavaScript, and runs on numerous platforms (tested for iOS).

It's based on [image-comparison-slider](https://github.com/CodyHouse/image-comparison-slider).

The app uses:

* Cordova: https://cordova.apache.org/
* jQuery Mobile: http://jquerymobile.com/

## Installation

Requires [Node.js](https://nodejs.org/)

```
sudo npm install -g cordova
sudo npm install -g cordova-icon
sudo npm install -g cordova-splash
cordova plugin add cordova-plugin-statusbar
cordova platform add ios
cordova run ios
```

## Building Native Apps

More info on how to use Cordova to build native apps for various platform can be found on the [Cordova CLI documentation](https://cordova.apache.org/docs/en/latest/guide/cli). Since this app is already structured as a cordova app, you can skip straight to [adding platforms](https://cordova.apache.org/docs/en/latest/guide/cli/#add-platforms).

To generate icons and splash-screens for added platforms, run:

```
cordova-icon
cordova-splash
```

## Development

For adjusting style, you can use SASS and Bourbon (http://bourbon.io/). 
In www folder run:

```
sudo gem install bourbon
cd scss
bourbon install
cd ../
sass --watch scss:css
```



