## GunUi elements
GunUi is a set of webcomponents that enables you - the frontend developer - to build complex - [Gun](https://github.com/amark/gun) - applications without writing any javascript

### How? 
Because every element handles its own peace of data. You 'link' an element to a certain 'data-point' by setting one or two attributes.

### But Why?
Because i think that building applications should be as simple as combining html elements and setting some attributes.

## GunUi-Button
`gunui-button` is a Gun wrapper around [`paper-button`](https://www.webcomponents.org/element/PolymerElements/paper-button/elements/paper-button)

## Purpose of `gunui-button`
* Visual control of a boolean value in your Gun data.
* Syncs the state of the button with changes in Gun
* ...and then some...Take a look at the [demo](https://stefdv.github.io/gunui-button/components/gunui-button/demo/index.html)

#### Requirements
* [Gun](https://github.com/amark/gun) loaded in your main document
* [gunui-base](https://github.com/Stefdv/gunui-base) in your main document

## (Bower) Install gunui-button
( When Polymer 3 arrives we can skip the bower part, but for now...)
```
bower install gunui-button --save
```

## Your main document
```
<!doctype html>
<html lang="en">
  <head>
    <!-- load Gun from somewhere ( required ) -->
    <script src="my_path_to_gun.js"></script>

    <!-- import gunui-base ( required )-->
    <link rel="import" href="/bower_components/gunui-base/gunui-base.html">

    <!-- import gunui-button -->
    <link rel="import" href="/bower_components/gunui-button/gunui-button.html">

  </head>
  <body>
    <gunui-base></gunui-base>

    <!-- somewhere in your app, or in a custom element -->
    <gunui-button soul="lights" prop="lights.1.state" key="on">Light 1</gunui-button>

  </body>
</html>
```
That's it. No javascript!

You now control the property in Gun!

## Now what?
Now you are ready to start building great apps with Gun but without having to write javascript :). Take a look at all the GunUi elements available.

## Demos
If you don't fully understand the purpose of gunui take a look at some of the GunUi elements.
### property elements
* [gunui-button](https://stefdv.github.io/gunui-button/components/gunui-button/demo/index.html) Visual control of a Boolean value in your Gun data
* [gunui-progress](https://stefdv.github.io/gunui-progress/components/gunui-progress/demo/index.html) Visualize a Numeric value in your Gun data
* [gunui-slider](https://stefdv.github.io/gunui-slider/components/gunui-slider/demo/index.html) Visual control of a Numeric value in your Gun data.

## Contact
I am not much of an e-mail reader, but please post issues and questions.
It would speed things up if you ping me in [gitter](https://gitter.im/amark/gun) @Stefdv 
