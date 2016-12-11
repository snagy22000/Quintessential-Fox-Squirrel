# encodeURI()

*A function that encodes a Uniform Resource Identifier (URI)*


Use encodeURI() when you need to encode a string to be used for any resource that uses URIs and needs certain characters to remain un-encoded. 

The most common use is encoding a string to be used as a Uniform Resource Locator (URL), such as a web address. 


## Syntax

Assumes a complete URI. The function encodes special characters, with the exception of the following, which have special meaning in the URI: `,`,  `/`, `?`, `:`, `@`, `&`, `=`, `+`, `$`, `#`. 

It accepts a single parameter, which is required, representing the URI to be encoded. 

```
		encodeURI(URI)
```



### Return Value

Returns a string representing the encoded URI. 



### Parameters

#### uri

*Required*. Contains the uri to be encoded. 



## Example 1

In the example below, a string with spaces is passed into the function to be encoded, since spaces are invalid characters in a valid URI.

```
		encodeURI("http://www.domain.com/file with spaces to be encoded.html")
		
		Returns:
		"http://www.domain.com/file%20with%20spaces%20to%20be%20encoded.html"

```


## Example 2 - Complex

In the example below we pass a string of characters and special characters to encodeURI() to illustrate how the encoding works. 

```
		encodeURI("~!@#$%^&*(){}[]=:/,;?+\'"\\")
		
		Returns: 
		"~!@#$%25%5E&*()%7B%7D%5B%5D=:/,;?+'%22%5C"
```

## Browser Support

### Desktop
| Chrome | Safari | Firefox | Internet Explorer | Opera |
|--------|--------|---------|-------------------|-------|
| Yes    | Yes    | Yes     | Yes               | Yes   | 

### Mobile
| Chrome | Safari | Firefox | Internet Explorer | Opera |
|--------|--------|---------|-------------------|-------|
| Yes    | Yes    | Yes     | Yes               | Yes   | 


## Special Notes

Note that encodeURIComponent() is often misunderstood as synonymous to encodeURI(). encodeURIComponent() encodes characters that will return a string that *will not be* a well-formed URL. 

For example: 
`encodeURI("http://www.domain.com/some spaces for resulting search#an-anchor")`

returns: 
`"http://www.domain.com/some%20spaces%20for%20resulting%20search#an-anchor"`

while: 
`encodeURIComponent("http://www.domain.com/some spaces for resulting search#an-anchor")`

returns: 
`"http%3A%2F%2Fwww.domain.com%2Fsome%20spaces%20for%20resulting%20search%23an-anchor"`

which is an ill-formed URL.
