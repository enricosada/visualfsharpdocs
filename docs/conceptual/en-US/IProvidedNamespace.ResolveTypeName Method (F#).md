# IProvidedNamespace.ResolveTypeName Method (F#)

Compilers call this method to query a type provider for a type name.

**Namespace/Module Path**: Microsoft.FSharp.Core.CompilerServices

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
abstract this.ResolveTypeName : string -> Type

// Usage:
iProvidedNamespace.ResolveTypeName (typeName)
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*typeName*
Type: [string](http://msdn.microsoft.com/en-us/library/12b97856-ec80-4f70-a018-afb0753f755a)







## Return Value

## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
Resolver should return a type called **name** in namespace **NamespaceName** or **null** if the type is unknown.


## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 4.0, Portable




## See Also
[CompilerServices.IProvidedNamespace Interface &#40;F&#35;&#41;](CompilerServices.IProvidedNamespace+Interface+28%F%2329%.md)

