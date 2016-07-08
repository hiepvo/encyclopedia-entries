#The Function of The `textarea` Element and Its Attribute

An HTML textarea is an oversized TextField.

The `<textarea>` tag defines a multi-line text input control.

A text area can hold an unlimited number of characters, and the text renders in a fixed-width font (usually Courier).

The size of a text area can be specified by the cols and rows attributes, or even better; through CSS' height and width properties.

ex.

**HTML textarea code:**

```
<textarea rows="4" cols="50">
This is textarea</textarea>
```



####Attributes

**autofocus**

- *value*: autofocus. The autofocus attribute is a boolean attribute.
- *description*: **New in HTML5**. Specifies that a text area should automatically get focus when the page loads
- *usage*: 

```
<textarea autofocus>
</textarea>
```
- Browser support: Chrome, IE 10.0, Firefox 4.0, Safari, Opera


**cols**

- *value*: number
- *description*: Specifies the visible width of a text area. Default value is 20.
- *usage*:

```
<textarea rows="4" cols="50">
</textarea>
```

- Browser support: Safari(Yes), IE(Yes), Firefox(Yes), Chrome(Yes), Opera(Yes)

**dirname**

- *value*: dir_name.dir
- *description*: The dirname attribute enables the submission of the directionality of the form control along with the value of the form control on form submission.

- *usage*:

```	
<input name="text" dirname="text.dir">
```

- *Browser support*: Chrome(Yes), IE(No), Firefox(No), Safari(Yes), Opera(Yes)

**disabled**

- *value*: disabled. The disabled attribute is a boolean attribute.
- *description*: Specifies that a text area should be disabled
- *usage*:

```
<textarea disabled>

```

- Browser support: Chrome(Yes), IE(Yes), Firefox(Yes), Safari(Yes), Opera(Yes)

**form**

- *value*: form_id
- *description*: **New in HTML5**. Specifies one or more forms the text area belongs to
- *usage*: 

```
<form action="demo_form.asp" id="myForm">
</form>
```

- *Browser support*: Chrome(Yes), IE(No), Firefox(Yes), Safari(Yes), Opera(Yes)

**maxlength**

- *value*: number
- *description*: **New in HTML5**. Specifies the maximum number of characters allowed in the text area
- *usage*:

```
<textarea maxlength="50">
Enter text here...
</textarea>
```
- *browser support*: Chrome(Yes), IE(10.0), Firefox(4.0), Safari(Yes), Opera(15.0)

**name**

- *value*: text
- *description*: Specifies a name for a text area
- *usage*:

```
  <textarea name="comment">Enter text here...</textarea>
```

- Browser support: Chrome(Yes), IE(No), Firefox(Yes), Safari(Yes), Opera(Yes)


**placeholder**

- *value*: text
- *description*: **New in HTML5**. Specifies a short hint that describes the expected value of a text area
- *usage*:

```
<textarea placeholder="Enter text here..."></textarea>
```

- *Browser support*: Chrome(yes), IE(10.0), Firefox(4.0), Safari(5.0), Opera(11.5)

**readonly**

- *value*: readonly
- *description*: Specifies that a text area should be read-only
- *usage*: 

```
<textarea readonly>
Read Only Text 
</textarea>
```
- *Browser support*:  Chrome(Yes), IE(Yes), Firefox(Yes), Safari(Yes), Opera(Yes)


**required**

- *value*: required
- *description*: **New in HTML5**. Specifies that a text area is required/must be filled out
- *usage*:

```
  <textarea name="comment" required></textarea>
 ```
- *Browser support*: Chrome(5.0), IE(10.0), Firefox(4.0), Safari(Not supported), Opera(yes)

**rows**
- *value*: number
- *description*: Specifies the visible number of lines in a text area
- *usage*: 

```
<textarea rows="4" cols="50">
</text>
```
- *Browser support*: Chrome(Yes), IE(Yes), Firefox(Yes), Safari(Yes), Opera(Yes)


**wrap**

- *value*: hard| soft
- *description*: Specifies how the text in a text area is to be wrapped when submitted in a form
- *usage*: 

```
<textarea rows="2" cols="20" wrap="hard">
</textarea>
```
- *Browser support*:  Chrome(Yes), IE(Yes), Firefox(Yes), Safari(Yes), Opera(Yes)
