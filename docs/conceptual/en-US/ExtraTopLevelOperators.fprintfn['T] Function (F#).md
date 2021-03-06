# ExtraTopLevelOperators.fprintfn<'T> Function (F#)

The fprintfn prints to a file using the given format, and add a newline.

**Namespace/Module Path:** Microsoft.FSharp.Core.ExtraTopLevelOperators

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
fprintfn : TextWriter -> TextWriterFormat<'T> -> 'T

// Usage:
fprintfn textWriter format
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*textWriter*
Type: **T:System.IO.TextWriter**


*format*
Type: [TextWriterFormat](http://msdn.microsoft.com/en-us/library/2080c4a5-7bdd-4a01-8e01-10b498af92de)**&lt;'T&gt;**




## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
This function is named **PrintFormatLineToTextWriter** in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.

**The following example demonstrates the use of fprintfn to print a listing of the contents of a directory to a specified file, directorylisting.txt.**
**[!CODE [FsCoreLib2#5](../CodeSnippet/VS_Snippets_Fsharp/fscorelib2/FSharp/fs/program.fs#5)]****The following example is similar to the previous except that it also demonstrates the use of specifiers to customize the output in the format string. For more information on format specifiers, see [Printf Module](http://msdn.microsoft.com/en-us/library/ea074733-6b5d-498c-ac88-7e4e0f8ded25).**
**[!CODE [FsCoreLib2#6](../CodeSnippet/VS_Snippets_Fsharp/fscorelib2/FSharp/fs/program.fs#6)]**
## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Core.ExtraTopLevelOperators Module &#40;F&#35;&#41;](Core.ExtraTopLevelOperators+Module+28%F%2329%.md)

[Microsoft.FSharp.Core Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Core+Namespace+28%F%2329%.md)

