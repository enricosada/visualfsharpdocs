# HashCompare.FastCompareTuple3<'T1,'T2,'T3> Function (F#)

A primitive entry point used by the F# compiler for optimization purposes.

**Namespace/Module Path:** Microsoft.FSharp.Core.LanguagePrimitives.HashCompare

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
FastCompareTuple3 : IComparer -> 'T1 * 'T2 * 'T3 -> 'T1 * 'T2 * 'T3 -> int

// Usage:
FastCompareTuple3 comparer tuple1 tuple2
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*comparer*
Type: **T:System.Collections.IComparer**


The comparer object.


*tuple1*
Type: **'T1 &#42; 'T2 &#42; 'T3**


The first tuple of three elements.


*tuple2*
Type: **'T1 &#42; 'T2 &#42; 'T3**


The second tuple of three elements.



**The result of the comparison.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
This function is for use by compiled F# code and should not be used directly.


## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[LanguagePrimitives.HashCompare Module &#40;F&#35;&#41;](LanguagePrimitives.HashCompare+Module+28%F%2329%.md)

[Core.LanguagePrimitives Module &#40;F&#35;&#41;](Core.LanguagePrimitives+Module+28%F%2329%.md)

