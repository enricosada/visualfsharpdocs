# Array.sort<'T> Function (F#)

Sorts the elements of an array, returning a new array. Elements are compared using [Operators.compare](http://msdn.microsoft.com/en-us/library/295e1320-0955-4c3d-ac31-288fa80a658c).

**Namespace/Module Path:** Microsoft.FSharp.Collections.Array

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
Array.sort : 'T [] -> 'T [] (requires comparison)

// Usage:
Array.sort array
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*array*
Type: **'T**[[]](http://msdn.microsoft.com/en-us/library/def20292-9aae-4596-9275-b94e594f8493)


The input array.



**The sorted array.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
This is not a stable sort. Therefore, the original order of equal elements might not be preserved. For a stable sort, consider using [Seq.sort](http://msdn.microsoft.com/en-us/library/327ea595-e77c-4529-b61e-8c6cbf5ec92e).

This function is named **Sort** in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.

**The following code illustrates the use of Array.sort.**
**[!CODE [FsArrays#37](../CodeSnippet/VS_Snippets_Fsharp/fsarrays/FSharp/fs/program.fs#37)]**
**Output**
**[|-2; 1; 4; 5; 8|]**
## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Collections.Array Module &#40;F&#35;&#41;](Collections.Array+Module+28%F%2329%.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections+Namespace+28%F%2329%.md)

