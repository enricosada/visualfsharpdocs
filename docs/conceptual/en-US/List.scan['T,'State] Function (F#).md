# List.scan<'T,'State> Function (F#)

Applies a function to each element of the collection, threading an accumulator argument through the computation. This function takes the second argument, and applies the function to it and the first element of the list. Then, it passes this result into the function along with the second element, and so on. Finally, it returns the list of intermediate results and the final result.

**Namespace/Module Path:** Microsoft.FSharp.Collections.List

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
List.scan : ('State -> 'T -> 'State) -> 'State -> 'T list -> 'State list

// Usage:
List.scan folder state list
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*folder*
Type: **'State -&gt; 'T -&gt; 'State**


The function to update the state given the input elements.


*state*
Type: **'State**


The initial state.


*list*
Type: **'T**[list](http://msdn.microsoft.com/en-us/library/c627b668-477b-4409-91ed-06d7f1b3e4a7)


The input list.



**The list of states.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
This function is named **Scan** in compiled assemblies. If you are accessing the function from a .NET language other than F#, or through reflection, use this name.

**The following code shows how to use List.scan.**
**[!CODE [FsLists#54](../CodeSnippet/VS_Snippets_Fsharp/fslists/FSharp/fs/program.fs#54)]**
**Output**
**Initial balance:**
**$   1122.73**
**Transaction   Balance**
**$   -100.00 $   1122.73**
**$    450.34 $   1022.73**
**$    -62.34 $   1473.07**
**$   -127.00 $   1410.73**
**$    -13.50 $   1283.73**
**$    -12.92 $   1270.23**
**Final balance:**
**$   1257.31**
## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Collections.List Module &#40;F&#35;&#41;](Collections.List+Module+28%F%2329%.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections+Namespace+28%F%2329%.md)

