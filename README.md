# SSGS - Smart and simple grid system in SCSS

## Features
- written in SCSS
- create grids on demand, on the fly
- fluid
- "dont overthink it" approach
- works in all browsers
- works on all devices
- lightweigt - 6kb
- super fast
- easy to use
- easy to modify
- comes with the mixins for even faster development
- free to use and abuse

## Demo
Please see demo.html **or:**
#### Online demo:
SOON

## Default column widths:
12 - 100%

11 - 91.667%

10 -  83.333%

9 - 75%

8 - 66.667%

7 - 58.333%

6 - 50%

5 - 41.667%

4 - 33.333%

3 - 25%

2 - 16.666%

1 - 8.333%

thirds - 33.333%, 66.667%

fourths - 25%, 50%, 70%

fifths - 20%, 40%, 60%, 80%

sixths - 16.666%, 33.333%, 50%, 66.667%, 83.333%

golden ratio - 61.803398875%, 38.196601125%

## Media queries
##### more than 1399px - widescreens
##### <= 1399px, >=1199 - widescreens
##### < 1199px , >= 960px smaller screens
##### < 959px , >= 768px tablets
##### < 767px mobile

## SCSS variables
`@row_wide_screen` - width of container > 1399px, default = 80% of the browser

`$row_1200-1400` - width of container between 1200 and 1399px, default = 90% of the browser

`$row_960-1200` - width of container between 960 and 1199px, default = 90% of the browser

`$row_tablet` - width of container between 768 and 959, default = 100% of the browser

`$gutter` - margin between columns, default = 1% (1% from left and 1% from right)

`$fw-gutter` - margin between columns in full-width grid, default = 1% (1% from left and 1% from right)

##### Mobile row is not a variable, its default value is 100%

##Options
`center` - centers any column

`right` - pull column right

`no-gutter` - removes the gutter between columns (goes on every column wanted to be guterless)

## Usage
### 1. Edit the grid.scss
Create your grid, define widths and gutter and you are ready to go! Simple as that. What else do you need?
### 2. Add SSGS grid to your project
##### Call via css
`<link rel="stylesheet" href="grid.css">`  **or:**
##### Copy CSS and add to your project
### 3. Add SSGS HTML
##### Names: 
`row` = container

`span-1` to `span-12` = columns from 1 to 12
##### HTML for normal row: 
```
<div class="row">

  <div class="span-12">grid 12</div>
  
  <div class="span-8">grid 8</div>
  <div class="span-4">grid 4</div>
  
  <div class="span-7">grid 7</div>
  <div class="span-5">grid 5</div>
  
  <div class="span-6">grid 6</div>
  <div class="span-6">grid 6</div>
  
  <div class="span-golden-big">Golden ratio grid big</div>
  <div class="span-golden-small">Golden ratio grid small</div>
  
  <div class="span-3">grid 3</div>
  <div class="span-3">grid 3</div>
  <div class="span-3">grid 3</div>
  <div class="span-3">grid 3</div>
  
</div>
```

##### HTML for full-width row: 
```
<div class="row-full-width">

  <div class="span-12">grid 12</div>
  
  <div class="span-8">grid 8</div>
  <div class="span-4">grid 4</div>
  
  <div class="span-7">grid 7</div>
  <div class="span-5">grid 5</div>
  
  <div class="span-6">grid 6</div>
  <div class="span-6">grid 6</div>
  
  <div class="span-golden-big">Golden ratio grid big</div>
  <div class="span-golden-small">Golden ratio grid small</div>
  
  <div class="span-3">grid 3</div>
  <div class="span-3">grid 3</div>
  <div class="span-3">grid 3</div>
  <div class="span-3">grid 3</div>
  
</div>
```

##### HTML for options usage:
```
<div class="row">

  <div class="span-8 center">column 8 centered</div>

  <div class="span-8 right">column 8 pulled right</div>

  <div class="span-4 no-gutter">column 4 without gutter</div>
  <div class="span-4 no-gutter">column 4 without gutter</div>
  <div class="span-4 no-gutter">column 4 without gutter</div>

</div>
```

## Mixins
Mixins `clearfix` and `breakpoints` are taken from my
sass-mixins repo.
Please check the syntax (they have same name) and usage
with demos there:
https://github.com/marioloncarek/sass-mixins


## Made with (thanks)
- [SASS](http://sass-lang.com/)
- [Codepen](http://codepen.io)
