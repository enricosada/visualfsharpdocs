# Lazy Computations (F#)

*Lazy computations* are computations that are not evaluated immediately, but are instead evaluated when the result is needed. This can help to improve the performance of your code.


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
let identifier = lazy ( expression )
```

## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
In the previous syntax, *expression* is code that is evaluated only when a result is required, and *identifier* is a value that stores the result. The value is of type [Lazy&lt;'T&gt;](http://msdn.microsoft.com/en-us/library/b29d0af5-6efb-4a55-a278-2662a4ecc489), where the actual type that is used for **'T** is determined from the result of the expression.

Lazy computations enable you to improve performance by restricting the execution of a computation to only those situations in which a result is needed.

To force the computation to be performed, you call the method **Force**. **Force** causes the execution to be performed only one time. Subsequent calls to **Force** return the same result, but do not execute any code.

The following code illustrates the use of lazy computation and the use of **Force**. In this code, the type of **result** is **Lazy&lt;int&gt;**, and the **Force** method returns an **int**.

[!CODE [FsLangRef2#73011](../CodeSnippet/VS_Snippets_Fsharp/fslangref2/FSharp/fs/lazy.fs#73011)]
    Lazy evaluation, but not the **Lazy** type, is also used for sequences. For more information, see [Sequences &#40;F&#35;&#41;](Sequences+28%F%2329%.md).


## See Also
[F&#35; Language Reference](F%23+Language+Reference.md)

[LazyExtensions module](http://msdn.microsoft.com/en-us/library/86671f40-84a0-402a-867d-ae596218d948)

