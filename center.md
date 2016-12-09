# HTML Element <center>

*horizontale centered HTML Element*

The Element is obsolet since HTML4. CSS Styles will be now used to center the content.

It was the shorthand for DIV align=center.


## Syntax

Introduction to the syntax/usage. A example of syntax is below:

    align = left|center|right|justify
    

| Meaning | Center elements horizontally. Short form for DIV align = center.      	|
|:-------------:|:-------------:	|
| Tags 	|  Start-Tag: required /  End-Tag: required  / <center>…</center>	|
| Parentelemente |  applet, blockquote, body, button, center, dd, del, div, fieldset, form, iframe, ins, li, map, noframes, noscript, object, td, th   	|

This attribute specifies the horizontal alignment of its element with respect to the surrounding context. Possible values:

    left: text lines are rendered flush left.
    center: text lines are centered.
    right: text lines are rendered flush right.
    justify: text lines are justified to both margins.
    
The default depends on the base text direction. For left to right text, the default is align=left, while for right to left text, the default is align=right.

Shorthand:
    
       <center> your content  </center>

#### url(path)

Example 1:
http://jsbin.com/nasogaxoze/3/edit?html,output

Example 2:
http://jsbin.com/redupajiqo/edit?html,output

## Example 1


        <center><h1>HTML Element</h1> 
        <p>The CENTER element is exactly equivalent to specifying the DIV element with the align attribute set to       "center". </p> 
        <p>The CENTER element is deprecated.</p> 
        <p>https://www.w3.org/TR/html401/present/graphics.html#edef-CENTER</p>
      </center>

## Example 2

DEPRECATED EXAMPLE: This example centers a heading on the canvas.

    <H1 align="center"> How Css Works </H1>
    
Using CSS, for example, you could achieve the same effect as follows:

    <HEAD>
     <TITLE>How CSS Works</TITLE>
     <STYLE type="text/css">
      H1 { text-align: center}
     </STYLE>
    <BODY>
     <H1>How CSS Works </H1>


## Example 3 - Complex

DEPRECATED EXAMPLE: 
Similarly, to right align a paragraph on the canvas with HTML's align attribute you could have:

    <P align="right">...Lots of loremipsum text...

which, with CSS, would be:

    <HEAD>
     <TITLE>How to Carve Wood</TITLE>
     <STYLE type="text/css">
      P.mypar {text-align: right}
     </STYLE>
    <BODY>
     <P class="mypar">...Lots of paragraph text...
 
DEPRECATED EXAMPLE: 
To right align a series of paragraphs, group them with the DIV element:

    <DIV align="right">
     <P>...text in first paragraph...
     <P>...text in second paragraph...
     <P>...text in third paragraph...
    </DIV>
    
With CSS, the text-align property is inherited from the parent element, you can therefore use:

    <HEAD>
     <TITLE>How CSS Works</TITLE>
     <STYLE type="text/css">
      DIV.mypars {text-align: right}
     </STYLE>
    <BODY>
     <DIV class="mypars">
      <P>...text in first paragraph...
      <P>...text in second paragraph...
      <P>...text in third paragraph...
     </DIV>    

To center the entire document with CSS:

    <HEAD>
     <TITLE>How CSS Works</TITLE>
     <STYLE type="text/css">
      BODY {text-align: center}
     </STYLE>
    <BODY>
     ...the body is centered...
    </BODY>

## Special Notes

The CENTER element is exactly equivalent to specifying the DIV element with the align attribute set to "center". The CENTER element is deprecated.
