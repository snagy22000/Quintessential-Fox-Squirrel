# CSS element element Selector

*The element element selector is used to select elements inside elements.*

Element Element Selectors or in CSS called "Descendant Selector" are using simple selectors to get a context relationship.

As an example, let’s say you want to style only those em elements that are descended from h1 elements. You could put a class attribute on every em element found within an h1, but that’s almost as time-consuming as using the font tag. It’s far more efficient to declare rules that match only em elements that are found inside h1 elements..

## Syntax

    selector1 selector2 { /* property declarations */ }

## Example 1

In the following example, all <em> elements that occur anywhere within <span> elements will have their text color set to green:

    span em { color:green; }

## Example 2

    body h1 {font-size: 200%;}
    table tr td div ul li {color: purple;}

## Example 3 - Complex

    div:not(.help) span {color: gray;}
    div.help span {color: red;}
    <div class="help">
        <div class="aside">
            This text contains <span>a span element</span> within.
        </div>
    </div>

Any span inside a div that doesn’t have a class containing the word help should be gray” in the first rule, and “any span inside a div whose class contains the word help” in the second rule. In the given markup fragment, both rules apply to the span shown.   

Because the two rules have equal weight and the “red” rule is written last, it wins out and the span is red. The fact that the div class="aside" is “closer to” the span than the div      class="help" is completely irrelevant. Again: descendant selectors have no notion of element proximity. Both rules match, only one color can be applied, and due to the way CSS works, red is the winner here.

## Special Notes

Descendant selectors can be extremely powerful. They make possible what could never be done in HTML—at least not without oodles of font tags.
