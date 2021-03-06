# FSharpValue.PreComputeUnionConstructorInfo Method (F#)

A method that constructs objects of the given case.

**Namespace/Module Path:** Microsoft.FSharp.Reflection

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
static member PreComputeUnionConstructorInfo : UnionCaseInfo * ?BindingFlags -> MethodInfo
static member PreComputeUnionConstructorInfo : UnionCaseInfo * ?bool -> MethodInfo

// Usage:
FSharpValue.PreComputeUnionConstructorInfo (unionCase)
FSharpValue.PreComputeUnionConstructorInfo (unionCase, bindingFlags = bindingFlags)

open FSharpReflectionExtensions;
FSharpValue.PreComputeUnionConstructorInfo (unionCase, allowAccessToPrivateRepresentation = false)
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*unionCase*
Type: [UnionCaseInfo](http://msdn.microsoft.com/en-us/library/d97eb038-9521-4e20-89b4-dd0cd92d7221)


The description of the union case.


*bindingFlags*
Type: **T:System.Reflection.BindingFlags**


Optional binding flags.


*allowAccessToPrivateRepresentation*
Type: [bool](http://msdn.microsoft.com/en-us/library/89c0cf9c-49ce-4207-a3be-555851a67dd5)


Optional flag that denotes accessibility of the private representation.



**The description of the constructor of the given union case as a T:System.Reflection.MethodInfo object.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]

## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Reflection.FSharpValue Class &#40;F&#35;&#41;](Reflection.FSharpValue+Class+28%F%2329%.md)

[Microsoft.FSharp.Reflection Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Reflection+Namespace+28%F%2329%.md)

