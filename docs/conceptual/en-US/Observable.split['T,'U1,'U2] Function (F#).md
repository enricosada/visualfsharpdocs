# Observable.split<'T,'U1,'U2> Function (F#)

Returns two observables which split the observations of the source by the given function. The first will trigger observations for which the splitter returns **Choice1Of2**. The second will trigger observations **y** for which the splitter returns **Choice2Of2**. The splitter is executed once for each subscribed observer. Both also propagate error observations arising from the source and each completes when the source completes.

**Namespace/Module Path**: Microsoft.FSharp.Control.Observable

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
Observable.split : ('T -> Choice<'U1,'U2>) -> IObservable<'T> -> IObservable<'U1> * IObservable<'U2>

// Usage:
Observable.split splitter source
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*splitter*
Type: **'T -&gt;**[Choice](http://msdn.microsoft.com/en-us/library/2ab2513e-e307-4360-96cd-8b682a8d64f0)**&lt;'U1,'U2&gt;**


The function that takes an observation and transforms it into one of the two output [Choice](http://msdn.microsoft.com/en-us/library/2ab2513e-e307-4360-96cd-8b682a8d64f0) types.


*source*
Type: [IObservable](http://msdn.microsoft.com/en-us/library/04855e2b-42e4-4342-860a-b86566c4f2d9)**&lt;'T&gt;**


The input Observable.



**A tuple of Observables. The first triggers when splitter returns Choice1of2 and the second triggers when splitter returns Choice2of2.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
This function is named **Split** in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.


## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Control.Observable Module &#40;F&#35;&#41;](Control.Observable+Module+28%F%2329%.md)

[Microsoft.FSharp.Control Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Control+Namespace+28%F%2329%.md)

