#HTML `script` tag


The HTML `script` element is a multi-line plain-text editing control.


## Syntax

```
	<script></script>

```

##Attributes

###async
Set this Boolean attribute to indicate that the browser should, if possible, execute the script asynchronously. It has no effect on inline scripts (i.e., scripts that don't have the src attribute).

###integrity
Contains inline metadata that a user agent can use to verify that a fetched resource has been delivered free of unexpected manipulation. 

###src
This attribute specifies the URI of an external script; this can be used as an alternative to embedding a script directly within a document. If a script element has a src attribute specified, it should not have a script embedded inside its tags.

###type
This attribute identifies the scripting language of code embedded within a script element or referenced via the element’s src attribute. This is specified as a MIME type; examples of supported MIME types include text/javascript, text/ecmascript, application/javascript, and application/ecmascript. If this attribute is absent, the script is treated as JavaScript.

###text
Like the textContent attribute, this attribute sets the text content of the element.  Unlike the textContent attribute, however, this attribute is evaluated as executable code after the node is inserted into the DOM.

###language 
Like the type attribute, this attribute identifies the scripting language in use. Unlike the type attribute, however, this attribute’s possible values were never standardized. The type attribute should be used instead.

###defer
This Boolean attribute is set to indicate to a browser that the script is meant to be executed after the document has been parsed. Since this feature hasn't yet been implemented by all other major browsers, authors should not assume that the script’s execution will actually be deferred. The defer attribute shouldn't be used on scripts that don't have the src attribute. Since Gecko 1.9.2, the defer attribute is ignored on scripts that don't have the src attribute. However, in Gecko 1.9.1 even inline scripts are deferred if the defer attribute is set.

###crossorigin 
Normal script elements pass minimal information to the window.onerror for scripts which do not pass the standard CORS checks. To allow error logging for sites which use a separate domain for static media, several browsers have enabled the crossorigin attribute for scripts using the same definition as the standard img crossorigin attribute. Efforts to standardize this attribute are underway on the WHATWG mailing list.

##Example

```
	<!-- HTML4 and (x)HTML -->
	<script type="text/javascript" src="javascript.js"></script>

	<!-- HTML5 -->
	<script src="javascript.js"></script>

```






