# Map.TryFind<'Key,'Value> Method (F#)

Lookup an element in the map, returning a **Some** value if the element is in the domain of the map and **None** if not.

**Namespace/Module Path:** Microsoft.FSharp.Collections

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
member this.TryFind : 'Key -> 'Value option (requires comparison)

// Usage:
map.TryFind (key)
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*key*
Type: **'Key**


The input key.



**The mapped value, or None if the key is not in the map.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
**The following code shows how to use the TryFind method.**
**[!CODE [FsMaps#16](../CodeSnippet/VS_Snippets_Fsharp/fsmaps/FSharp/fs/program.fs#16)]**
**Output**
**Found 2500.**
## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Collections.Map&#60;'Key,'Value&#62; Class &#40;F&#35;&#41;](Collections.Map%3C%27Key%2C%27Value%3E+Class+28%F%2329%.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections+Namespace+28%F%2329%.md)

