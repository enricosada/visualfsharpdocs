# Async.CancellationToken Property (F#)

Creates an asynchronous computation that returns the cancellation token governing the execution of the computation.

**Namespace/Module Path:** Microsoft.FSharp.Control

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
static member CancellationToken :  Async<CancellationToken>

// Usage:
Async.CancellationToken
```
**An asynchronous computation capable of retrieving the T:System.Threading.CancellationToken from a computation expression.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
In an asynchronous computation such as the following, a cancellation token can be used to initiate other asynchronous operations that will cancel cooperatively with this workflow.


```f#
async { let! token = Async.CancellationToken ...}
```

## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Control.Async Class &#40;F&#35;&#41;](Control.Async+Class+28%F%2329%.md)

[Microsoft.FSharp.Control Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Control+Namespace+28%F%2329%.md)

