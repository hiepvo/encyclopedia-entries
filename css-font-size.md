#CSS font-size Property


The font-size CSS property specifies the size of the font.


## Syntax



```
font-size: <medium |xx-small | x-small | small | large | x-large | xx-large | smaller | larger | length | initial | inherit>;

```

### Values


#### xx-small, x-small, small, medium, large, x-large, xx-large

A set of absolute size keywords based on the user's default font size (which is medium). 

#### larger, smaller

Larger or smaller than the parent element's font size, by roughly the ratio used to separate the absolute size keywords above.


#### length

A positive `<length>`. When the units are specified in em or ex, the size is defined relative to the size of the font on the parent element of the element in question. For example, 0.5em is half the font size of the parent of the current element. When the units are specified in rem, the size is defined relative to the size of the font used by the html (root) element.

####percentage

A positive `<percentage>` of the parent element's font size.

####maxlength

Specifies the maximum number of characters allowed in the text area

####name

Specifies a name for a text area

####placeholder

Specifies a short hint that describes the expected value of a text area

####readonly

Specifies that a text area should be read-only

####required

Specifies that a text area is required/must be filled out

####rows

Specifies the visible number of lines in a text area

####wrap

Specifies how the text in a text area is to be wrapped when submitted in a form

##Approaches
There are several ways to specify the font size, with keywords or numerical values for pixels or ems. Choose the appropriate method based on the needs for the particular web page.

###Keywords
Keywords are a good way to set the size of fonts on the web. By setting a keyword font size on the body element, you can set relative font-sizing everywhere else on the page, giving you the ability to easily scale the font up or down on the entire page accordingly.

##Pixels
Setting the font size in pixel values (px) is a good choice when you need pixel accuracy. A px value is static. This is an OS-independent and cross-browser way of literally telling the browsers to render the letters at exactly the number of pixels in height that you specified. The results may vary slightly across browsers, as they may use different algorithms to achieve a similar effect.

##Ems

Another way of setting the font size is with em values. The size of an em value is dynamic. When defining the font-size property, an em is equal to the size of the font that applies to the parent of the element in question. If you haven't set the font size anywhere on the page, then it is the browser default, which is probably 16px. So, by default 1em = 16px, and 2em = 32px. If you set a font-size of 20px on the body element, then 1em = 20px and 2em = 40px. Note that the value 2 is essentially a multiplier of the current em size.

##Rems

rem values were invented in order to sidestep the compounding problem. rem values are relative to the root html element, not the parent element. In other words, it lets you specify a font size in a relative fashion without being affected by the size of the parent, thereby eliminating compounding.

##Example 1

```
/* Set paragraph text to be very large. */
p { font-size: xx-large }

/* Set h1 (level 1 heading) text to be 2.5 times the size
 * of the text around it. */
h1 { font-size: 250% }

/* Sets text enclosed within span tag to be 16px */
span { font-size: 16px; }

```

##Example 2

```
.small {
	font-size: xx-small;
}
.larger {
	font-size: larger;
}
.point {
	font-size: 24pt;
}
.percent {
	font-size: 200%;
}

```

##Example 2

```
span {
  font-size: 1.6em; /* 1.6em = 16px */
}

span {
  font-size: 1.6rem;
}

```

##Special Notes

em and ex units on the font-size property are relative to the parent element's font size (unlike all other properties, where they're relative to the font size on the element). This means em units and percentages do the same thing for font-size.