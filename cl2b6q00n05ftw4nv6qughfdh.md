## Type Conversion

In the previous blog, I covered the data types and some other important concepts in a JAVA program. If you have not read my previous blog yet then click [here](https://clevercoderjoy.hashnode.dev/data-types-in-java-by-clevercoderjoy) to give it a read and then proceed further from here. If you want to get started with JAVA for the first time then you should start reading my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) in the JAVA series.

In this blog, I will walk you through type conversion and some important key points around the concept.

# Type Conversion

The conversion of one data type into another data type is called type conversion.
When one type of data is assigned to another type of variable, then automatic type conversion will take place if the following conditions are met:
- The two types should be compatible (String and characters are not compatible with int, float, and long).
- The destination type should be greater than the source type (taking an integer and providing a float or a decimal value as an input will result in an error but vice versa will work).
- JAVA also performs automatic type conversion when storing integer constants into variables of types like byte, short, long, and even char sometimes by using their ASCII values.

# Type Casting

- If the destination type is smaller than the source, then that type of conversion is also called type casting or narrowing conversion.
- Simply put, compressing the bigger number into a smaller data type explicitly is called type casting.
- Type casting is also known as coercion.
- If we have multiple types of data for a particular expression, then the result for the entire expression will be converted into the biggest data type.

> JAVA follows Unicode principles so we can put any language inside it to print it via ``` System.out.print("any language"); ```

This is all about type casting and type conversion in JAVA. I hope that you will be able to understand everything very well.

In the next blog, I will cover loops and conditionals in a JAVA program in the next blog.

Let me know comments down below if you like what you read or have some suggestions for me and make sure to follow me on all my social handles from [here](https://clevercoderjoy.bio.link/) to stay connected. If you want to get started with JAVA for the first time then you can hop back to my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) of this series.
