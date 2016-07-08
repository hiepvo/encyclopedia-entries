#The resize property in CSS3

CSS3 offers new feature in CSS3 User interface section: the resize property. It allows you to specify if a box is resizable.

Textarea resizing is hugely helpful when you're looking to post a long message.

HTML

```
<textarea class="resize-both">Type some text here.</textarea>
```

CSS

```
.resize-both { 
		resize: both; 
		overflow: auto; 
		}
```

If you want to constrain the width and height of the textarea element, these browsers also respect max-height, `max-width`, `min-height`, and `min-width` CSS properties to provide resizing:

```
.resize-both { 
		resize: both; 
		overflow: auto; 
		max-width: 300px;
		min-width: 150px;
		}
```




**Note**:
- resize does nothing unless the overflow property is set to something other than visible, which is its initial value for most elements.
- Firefox let you resize an element smaller than its original size.
- Webkit browsers will not let you resize an element to make it smaller, only larger (in both dimiensions)


####values

**none**: The element offers no user-controllable method for resizing the element.

**both**: The element displays a mechanism for allowing the user to resize the element, which may be resized both horizontally and vertically.

**horizontal**: The element displays a mechanism for allowing the user to resize the element, which may only be resized horizontally.

**vertical**: The element displays a mechanism for allowing the user to resize the element, which may only be resized vertically.

**block**: Depending on the writing-mode and direction value, the element displays a mechanism for allowing the user to resize the element either horizontally or vertically in block direction.]

**inline**: Depending on the writing-mode and direction value, the element displays a mechanism for allowing the user to resize the element either horizontally or vertically in inline direction.

####Browser support:

- Chrome: 4+
- Safari: 7+
- Firefox: 4+
- Opera: 30+
- IE: None
