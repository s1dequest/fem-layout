d# CSS Grid and Flexbox Fundamentals & Practice
**Based on the FrontendMasters course by Jen Kramer**  

## Outline:
Starting with a review of floats for context, but quickly moving into Flexbox and CSS grids,  
this essential course is for web developers that want to build responsive, beautiful web applications  
faster using less code and best practices. Master CSS Grid and Flexbox, the latest tools and  
tricks to layout beautiful, responsive web applications with less code.  
  
Other misc stuff from the intro:
* CSS3 Media Queries:
  * Basically, your browser reports screen resolution. This indicates screen size (width). From that width the website determines what stylesheet & layout to use for that width.
  * No JS involved with this.

## Floats:
Basically, a hack for layout.
* They were just intended to float images.  
* Rows and cells.
* Rows 'clear' the floats on the cells. "If you float, you must clear."
* Source ordering determines display on the page, generally. I.E. what ordering your HTML is in, will be the order in which they appear on screen.
* Biggest disadvantage: Equal column heights.
```html One row with 4 columns.
<div class="row">
  <div class="col-1"></div>
  <div class="col-1"></div>
  <div class="col-1"></div>
  <div class="col-1"></div>
</div>
```
```css for above.
.row::after { /*How to clear a row.*/
  content: "";
  display: table;
  clear: both;
}
.col-1 {
  float: left;
  margin-left: 4%;
  width: 20%;
}
```
* Wrapping via Media Query: (2 rows of 2)
```css for above.
@media only screen and (min-width: 480px)
                   and (max-width: 767px) {
  .col-1 {
    width: 44%;
  }
}
```
* 4 Rows of 1:
```css for above.
@media only screen and (max-width: 479px) {
  .col-1 {
    width: 98%;
    margin: 1%;
    float: none;
  }
}
```
This becomes a mess.  
I'm not going to take many notes on these. As I expect they won't be very useful.

## Flexbox:

## Flexbox Grid:

## Exercises:

## Responsive Images:

## CSS Grid:

