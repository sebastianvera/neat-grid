Neat Grid
=========

Bourbon's Neat grid classes because you need them for some reason

Note
----
This tiny set of classes will go against Neat's premise, which is to keep grid logic out of the HTML markup.

You should NOT use this if
--------------------------
Your app is not currently Bourbon-dependant and you do not need a class-based grid system.

Here are some useful grid systems you can look at:

- [960 Grid system](http://960.gs/)
- [Simple Grid](http://thisisdallas.github.io/Simple-Grid/)
- [Wizardry Grids](http://csswizardry.com/csswizardry-grids/)


Why/When to use this
--------------------
Class based grid systems are actually quite great, they allow you to easily change the visual structure of your project without having to touch both CSS and HTML for every change. Also, they strongly prevent css style repetition. I'd suggest to use this set of classes if you like how Bourbon works and it's a must have in your project. If maybe you are following a module-focused CSS structure like [SMACSS](http://smacss.com/) or you are using a strongly HTML focused front-end framework like [AngularJs](https://angularjs.org/) or [KnockoutJs](http://knockoutjs.com/).

Installing
============
At your main .scss file import the bourbon, neat, and neat-grid libraries in that order

Bower
-----
```
bower install neat-grid
```

```scss
@import 'bower_components/bourbon/dist/bourbon';
@import 'bower_components/neat/app/assets/stylesheets/neat';
@import 'bower_components/neat-grid/neat-grid';

```

Manually
--------
Copy the neat-grid.scss file to your project, make sure you have bourbon and neat installed.

Then import the files in your main .scss
```scss
@import 'path/to/bourbon';
@import 'path/to/neat';
@import 'path/to/neat-grid';
```

How to use
==========
Neat Grid is a quite simple set of classes to define columns in your HTML.

A common set of columns
```html
<section class="grid-wrap">
  <div class="grid-6">This is half of the grid space</div>
  <div class="grid-3">This is 1/4 of the grid space</div>
  <div class="grid-2">This is 1/6 of the grid space</div>
  <div class="grid-1">This is 1/12 of the grid space</div>
</section>
```

Nested columns
```html
<section class="grid-wrap">
  <div class="grid-6">
    <div class="grid-2-6">This uses 2 out 6 columns from the parent</div>
    <div class="grid-4-6">This uses 4 out of 6 columns from the parent</div>
  </div>
  
  <div class="grid-6">
    Common column using half of the grid
  </div>
</section>
```
