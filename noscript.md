# <noscript>

*Defines alternate HTML for users that have scripts disabled *

Use noscript when you want your program to degrade gracefully. It can be used in both `<head>` and `<body>`.  


## Syntax

```
		<noscript>Alternate HTML</noscript>
```



## Example 1

The example below prints additional content when scripting is disabled. 

```
		<noscript>
			<p>This text will only appear with scripting disabled.</p>
		</noscript>
		<p>This text will always appear.</p>
		
```



### Result with Scripting Enabled

```
This text will always appear.
```



### Result with Scripting Disabled

```
This text will only appear with scripting disabled. 

This text will always appear. 
```



## Example 3 - Complex

In the example below a link is shown when scripting is disabled. 

```
<!doctype html>
<html>

<head>
<meta charset="UTF-8">
<title>Example of noscript html element</title>
</head>

<body>
<h1>This heading is always shown.</h1>
<p>This paragraph is always shown.</p>
<script src="/js/example.js"></script>
<noscript>
  <p><a href="examples.html">This link is shown only if scripting is disabled.</a></p>
</noscript>
</body>
</html>
```



### Results with Scripting Enabled



## This heading is always shown.

This paragraph is always shown. 



### Results with Scripting Disabled



## This heading is always shown.

This paragraph is always shown. 



<u>This link is shown only if scripting is disabled.</u> 



## Browser Support

### Desktop

| Chrome | Safari | Firefox | Internet Explorer | Opera |
| ------ | ------ | ------- | ----------------- | ----- |
| Yes    | Yes    | Yes     | Yes               | Yes   |

### Mobile

| Chrome | Safari | Firefox | Internet Explorer | Opera |
| ------ | ------ | ------- | ----------------- | ----- |
| Yes    | Yes    | Yes     | Yes               | Yes   |





## Special Notes

The `noscript` element only detects whether JavaScript is enabled or not at the browser level. If JavaScript is disabled at the firewall level, for example, then the content of `noscript` will not be displayed. 



The `noscript` element is a block-level element and cannot be used inline. 

