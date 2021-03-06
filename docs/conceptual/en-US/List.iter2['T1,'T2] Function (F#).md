# List.iter2<'T1,'T2> Function (F#)

Applies the given function to two collections simultaneously. The collections must have identical size.

**Namespace/Module Path:** Microsoft.FSharp.Collections.List

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
List.iter2 : ('T1 -> 'T2 -> unit) -> 'T1 list -> 'T2 list -> unit

// Usage:
List.iter2 action list1 list2
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*action*
Type: **'T1 -&gt; 'T2 -&gt;**[unit](http://msdn.microsoft.com/en-us/library/00b837c2-6c8a-483a-87d3-0479c64037a7)


The function to apply to pairs of elements from the input lists.


*list1*
Type: **'T1**[list](http://msdn.microsoft.com/en-us/library/c627b668-477b-4409-91ed-06d7f1b3e4a7)


The first input list.


*list2*
Type: **'T2**[list](http://msdn.microsoft.com/en-us/library/c627b668-477b-4409-91ed-06d7f1b3e4a7)


The second input list.



**exceptions tag is not supported!!!!**

## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
This function is named **Iterate2** in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.

**The following code example illustrates the use of List.iter2 and compares its behavior with related functions.**
**[!CODE [FsLists#17](../CodeSnippet/VS_Snippets_Fsharp/fslists/FSharp/fs/program.fs#17)]**
**Output**
**List.iter: element is 1**
**List.iter: element is 2**
**List.iter: element is 3**
**List.iteri: element 0 is 1**
**List.iteri: element 1 is 2**
**List.iteri: element 2 is 3**
**List.iter2: elements are 1 4**
**List.iter2: elements are 2 5**
**List.iter2: elements are 3 6**
**List.iteri2: element 0 of list1 is 1 element 0 of list2 is 4**
**List.iteri2: element 1 of list1 is 2 element 1 of list2 is 5**
**List.iteri2: element 2 of list1 is 3 element 2 of list2 is 6**
## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Collections.List Module &#40;F&#35;&#41;](Collections.List+Module+28%F%2329%.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections+Namespace+28%F%2329%.md)

