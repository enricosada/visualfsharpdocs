# Array2D.init<'T> Function (F#)

Creates an array given the dimensions and a generator function to compute the elements.

**Namespace/Module Path**: Microsoft.FSharp.Collections.Array2D

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
Array2D.init : int -> int -> (int -> int -> 'T) -> 'T [,]

// Usage:
Array2D.init length1 length2 initializer
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*length1*
Type: [int](http://msdn.microsoft.com/en-us/library/025d5455-3622-4ea5-9573-3ecbd4ee1375)


The length of the first dimension of the array.


*length2*
Type: [int](http://msdn.microsoft.com/en-us/library/025d5455-3622-4ea5-9573-3ecbd4ee1375)


The length of the second dimension of the array.


*initializer*
Type: [int](http://msdn.microsoft.com/en-us/library/025d5455-3622-4ea5-9573-3ecbd4ee1375)**-&gt;**[int](http://msdn.microsoft.com/en-us/library/025d5455-3622-4ea5-9573-3ecbd4ee1375)**-&gt; 'T**


A function to produce elements of the array given the two indices.



**exceptions tag is not supported!!!!**
**The generated array.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
This function is named **Initialize** in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.

**The following code demonstrates the use of Array2D.init to create a two-dimensional array.**
**[!CODE [FsArrays#21](../CodeSnippet/VS_Snippets_Fsharp/fsarrays/FSharp/fs/program.fs#21)]**
## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Collections.Array2D Module &#40;F&#35;&#41;](Collections.Array2D+Module+28%F%2329%.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections+Namespace+28%F%2329%.md)

