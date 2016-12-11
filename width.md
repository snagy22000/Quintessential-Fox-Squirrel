# Width

*CSS property that specifies the width of the content area of an element.*

Along with `height` use `width` to set the dimensions of an element. You can specify `width` using pixels (px), centimeters (cm) or percentages (%) of the containing element.


## Syntax

Introduction to the syntax/usage. A example of CSS syntax is below:

```
		width: [<length> | <percentage>] && [border-box | content-box]? | available | min-content | max-content | fit-content | auto;
```

### Values

#### <length>

Denotes a distance measurement. It is a number followed by a length unit. 

| Unit Type                 | Units                     |
| ------------------------- | ------------------------- |
| Relative-length Units     | em, ex, ch, rem           |
| Viewport-percentage Units | vh, vw, vmin, vmax        |
| Absolute units            | px, mn, q, cm, in, pt, pc |

#### <percentage>

Width is calculated as a percentage of the containing element. 

#### border-box

If set, applies the width to the element's border box. 

#### content-box

*Default*. Applies the width to the element's content box

#### auto

*Default value*. The browser calculates `width` automatically. 

#### fill

Use the fill-available inline size or fill-available block size, as appropriate to the writing mode. 

#### max-content

The intrinsic preferred width. 

#### min-content

The intrinsic minimum width

#### available

The containing block width minus horizontal margin, border and padding. 

#### fit-content

The larger of: the instrinsic minimum width or the smaller of the intrinsic preferred width and the available width.

## 

## Example 1 - Pixels

In this example we set a `div` element's width using `px` units.

```
		.px_width {
            width: 200px;
            background-color: red;
            color: white;
            border: 1px solid black;
		}
		
```

```
	<div class="px_width">Div with 200px width</div>
```



![pixel width example](px-width.png)

## Example 2 - Percentage

In the following example we set the width of the `div` to 50% of the containing element. 

```
		.percent_width {
            width: 50%;
            background-color: red;
            color: white;
            border: 1px solid black;
		}
```



```
	<div class="percent_width">Div with 50% width</div>
```



Result: 

![percent width example](px-width.png)



## Example 3 - Complex

In the example below we use the little known `fit-content` value to set the containing element width based on the content. The `ul` element's width will adjust based on the content width of the `li` elements within it. 

```
ul {
  background: deepskyblue;
  padding: 1em;
  width: fit-content;

}

li {
  display: inline-block;
  background: red;
  padding: .5em;
}
```

Result: 

![Complex Example for Width](./width-article.png)

## Browser Support

### Desktop

| Chrome | Safari | Firefox | Internet Explorer | Opera |
| ------ | ------ | ------- | ----------------- | ----- |
| Yes    | Yes    | Yes     | Yes               | Yes   |

### Mobile

| Chrome | Safari | Firefox | Internet Explorer | Opera |
| ------ | ------ | ------- | ----------------- | ----- |
| Yes    | ?      | ?       | ?                 | ?     |



## Special Notes

The `min-width` and `max-width` properties override the `width` property. 

