# Core.FSharpInterfaceDataVersionAttribute Class (F#)

This attribute is added to generated assemblies to indicate the version of the data schema used to encode additional F# specific information in the resource attached to compiled F# libraries.

**Namespace/Module Path:** Microsoft.FSharp.Core

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
[<AttributeUsage(AttributeTargets.Assembly, AllowMultiple = false)>]
[<Sealed>]
type FSharpInterfaceDataVersionAttribute =
class
new FSharpInterfaceDataVersionAttribute : int * int * int -> FSharpInterfaceDataVersionAttribute
member this.Major :  int
member this.Minor :  int
member this.Release :  int
end
```

## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
You can also use the short form of the name, **FSharpInterfaceDataVersion**.


## Constructors


|Member|Description|
|------|-----------|
|[new](http://msdn.microsoft.com/en-us/library/2ea3742d-ef71-4db0-a8cc-ba682f582703)|Creates an instance of the attribute|

## Instance Members


|Member|Description|
|------|-----------|
|[Major](http://msdn.microsoft.com/en-us/library/e4412901-f87a-4374-a841-ecb8a9b18276)|The major version number of the F# version associated with the attribute|
|[Minor](http://msdn.microsoft.com/en-us/library/bd90b482-658f-400f-a920-71069ac37cca)|The minor version number of the F# version associated with the attribute|
|[Release](http://msdn.microsoft.com/en-us/library/0444826b-5338-482b-a04c-c72c0c5ac0fc)|The release number of the F# version associated with the attribute|

## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Microsoft.FSharp.Core Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Core+Namespace+28%F%2329%.md)

