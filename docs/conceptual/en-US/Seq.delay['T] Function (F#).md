# Seq.delay<'T> Function (F#)

Returns a sequence that is built from the given delayed specification of a sequence.

**Namespace/Module Path**: Microsoft.FSharp.Collections.Seq

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
Seq.delay : (unit -> seq<'T>) -> seq<'T>

// Usage:
Seq.delay generator
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*generator*
Type: [unit](http://msdn.microsoft.com/en-us/library/00b837c2-6c8a-483a-87d3-0479c64037a7)**-&gt;**[seq](http://msdn.microsoft.com/en-us/library/2f0c87c6-8a0d-4d33-92a6-10d1d037ce75)**&lt;'T&gt;**


The generating function for the sequence.



**The resulting sequence.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
The input function is evaluated each time an **IEnumerator** for the sequence is requested.

This function is named **Delay** in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.

**The following code shows how to use Seq.delay to delay the evaluation of a sequence that is created from a collection that is normally evaluated immediately.**
**[!CODE [FsSequences#30](../CodeSnippet/VS_Snippets_Fsharp/fssequences/FSharp/fs/program.fs#30)]**
**Output**
**Calling makeSequence.**
**Printing sequences.**
**Squares:**
**Evaluating 4.**
**Evaluating 3.**
**Evaluating 2.**
**Evaluating 1.**
**Evaluating 0.16 9 4 1 Cubes:Evaluating 4.**
**Evaluating 3.**
**Evaluating 2.**
**Evaluating 1.**
**Evaluating 0.**
**64 27 8 1****The following code example is equivalent to the previous example, except that it does not use Seq.delay. Notice the difference in the output.**
**[!CODE [FsSequences#31](../CodeSnippet/VS_Snippets_Fsharp/fssequences/FSharp/fs/program.fs#31)]**
**Output**
**Calling makeSequence.**
**Evaluating 4.**
**Evaluating 3.**
**Evaluating 2.**
**Evaluating 1.**
**Evaluating 0.**
**Evaluating 4.**
**Evaluating 3.**
**Evaluating 2.**
**Evaluating 1.**
**Evaluating 0.**
**Printing sequences.**
**Squares:**
**16 9 4 1**
**Cubes:**
**64 27 8 1**
## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Collections.Seq Module &#40;F&#35;&#41;](Collections.Seq+Module+28%F%2329%.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections+Namespace+28%F%2329%.md)

