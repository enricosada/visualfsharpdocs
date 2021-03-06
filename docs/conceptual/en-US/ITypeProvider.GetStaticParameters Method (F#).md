# ITypeProvider.GetStaticParameters Method (F#)

Get the static parameters for a provided type.

**Namespace/Module Path**: Microsoft.FSharp.Core.CompilerServices

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
abstract this.GetStaticParameters : Type -> ParameterInfo []

// Usage:
iTypeProvider.GetStaticParameters (typeWithoutArguments)
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*typeWithoutArguments*
Type: **T:System.Type**


A type returned by GetTypes or ResolveTypeName




## Return Value
An array of parameters.


## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 4.0Supported in: 4.0, Portable




## See Also
[CompilerServices.ITypeProvider Interface &#40;F&#35;&#41;](CompilerServices.ITypeProvider+Interface+28%F%2329%.md)

[Microsoft.FSharp.Core.CompilerServices Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Core.CompilerServices+Namespace+28%F%2329%.md)

