# CancellationToken.( <> ) Method (F#)

Inequality operator for tokens.

**Namespace/Module Path**: System.Threading

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
static member ( <> ) : CancellationToken * CancellationToken -> bool

// Usage:
token1 <> token2
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*token1*
Type: [CancellationToken](http://msdn.microsoft.com/en-us/library/31a3eafe-b61b-46c4-927d-bc9a3ae357c2)


*token2*
Type: [CancellationToken](http://msdn.microsoft.com/en-us/library/31a3eafe-b61b-46c4-927d-bc9a3ae357c2)



**False if the two tokens are equal.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
This API is provided for use only with the F# Core Library Versions that targets .NET Framework 2.0. If you are using .NET Framework 4, use the .NET Framework 4 API with the same name, **M:System.Threading.CancellationToken.op_Inequality(System.Threading.CancellationToken,System.Threading.CancellationToken)**.


## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0




## See Also
[Threading.CancellationToken Structure &#40;F&#35;&#41;](Threading.CancellationToken+Structure+28%F%2329%.md)

[System.Threading Namespace &#40;F&#35;&#41;](System.Threading+Namespace+28%F%2329%.md)

