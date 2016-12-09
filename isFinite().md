

# isFinite()

*To determine if a value is finite*

The isFinite () function determines whether a value is in the range of numbers that JavaScript can handle, also determines a valid number from JavaScript.

Returns true if the value is a valid number, and false if it is not a number or the number is outside the range of JavaScript. Both integers and commas are recognized as valid numbers. For commas, the decimal point must be a period.


## Syntax

    isFinite(Number)
    
Parameters:

    Number
    
The value to be tested for finiteness.

This function returns true only if the argument is between the minimum and the maximum values. 

## Example 1

    var result = Number.MAX_VALUE + Number.MAX_VALUE;
    alert(isFinite(result)); //false

Though it is rare to do calculations that take values outside of the range of finite numbers, it is possible and should be monitored when doing very large or very small calculations.

## Example 2

    var Number = Number.MAX_VALUE;
        if (!isFinite(Number * 2)) alert("The Number can not be processed");

The example defines a variable number that is assigned the largest possible number as the value Number.MAX_VALUE. The subsequent query checks whether the product of this number with 2 is within the processable range of numbers. If this is not the case, a corresponding warning message is issued.    

## Example 3 - Complex

    isFinite(Infinity);  // false
    isFinite(NaN);       // false
    isFinite(-Infinity); // false
    
    isFinite(0);         // true
    isFinite(2e64);      // true
    isFinite(null);      // true
    
    
    isFinite("0");       // true, would've been false with the 
                         // more robust Number.isFinite("0")

## Special Notes

Add information that you found that seemed lesser known. Common bugs, obscure bugs, important distinctions, all belong in this section.
