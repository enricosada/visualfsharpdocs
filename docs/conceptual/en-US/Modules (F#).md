# Modules (F#)

In the context of the F# language, a *module* is a grouping of F# code, such as values, types, and function values, in an F# program. Grouping code in modules helps keep related code together and helps avoid name conflicts in your program.


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Top-level module declaration. 
module [accessibility-modifier] [qualified-namespace.]module-namedeclarations
// Local module declaration.
module [accessibility-modifier] module-name =
declarations
```

## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
An F# module is a grouping of F# code constructs such as types, values, function values, and code in **do** bindings. It is implemented as a common language runtime (CLR) class that has only static members. There are two types of module declarations, depending on whether the whole file is included in the module: a top-level module declaration and a local module declaration. A top-level module declaration includes the whole file in the module. A top-level module declaration can appear only as the first declaration in a file.

In the syntax for the top-level module declaration, the optional *qualified-namespace* is the sequence of nested namespace names that contains the module. The qualified namespace does not have to be previously declared.

You do not have to indent declarations in a top-level module. You do have to indent all declarations in local modules. In a local module declaration, only the declarations that are indented under that module declaration are part of the module.

If a code file does not begin with a top-level module declaration or a namespace declaration, the whole contents of the file, including any local modules, becomes part of an implicitly created top-level module that has the same name as the file, without the extension, with the first letter converted to uppercase. For example, consider the following file.

[!CODE [FsModules#6601](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules1.fs#6601)]
    This file would be compiled as if it were written in this manner:

[!CODE [FsModules#6602](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules2.fs#6602)]
    If you have multiple modules in a file, you must use a local module declaration for each module. If an enclosing namespace is declared, these modules are part of the enclosing namespace. If an enclosing namespace is not declared, the modules become part of the implicitly created top-level module. The following code example shows a code file that contains multiple modules. The compiler implicitly creates a top-level module named **Multiplemodules**, and **MyModule1** and **MyModule2** are nested in that top-level module.

[!CODE [FsModules#6603](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules3.fs#6603)]
    If you have multiple files in a project or in a single compilation, or if you are building a library, you must include a namespace declaration or module declaration at the top of the file. The F# compiler only determines a module name implicitly when there is only one file in a project or compilation command line, and you are creating an application.

The *accessibility-modifier* can be one of the following: **public**, **private**, **internal**. For more information, see [Access Control &#40;F&#35;&#41;](Access+Control+28%F%2329%.md). The default is public.


## Referencing Code in Modules
When you reference functions, types, and values from another module, you must either use a qualified name or open the module. If you use a qualified name, you must specify the namespaces, the module, and the identifier for the program element you want. You separate each part of the qualified path with a dot (.), as follows.

**Namespace1.Namespace2.ModuleName.Identifier**

You can open the module or one or more of the namespaces to simplify the code. For more information about opening namespaces and modules, see [Import Declarations: The open Keyword &#40;F&#35;&#41;](Import+Declarations%3A+The+open+Keyword+28%F%2329%.md).

The following code example shows a top-level module that contains all the code up to the end of the file.

[!CODE [FsModules#6604](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules4.fs#6604)]
    To use this code from another file in the same project, you either use qualified names or you open the module before you use the functions, as shown in the following examples.

[!CODE [FsModules#6605](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules5.fs#6605)]
    
## Nested Modules
Modules can be nested. Inner modules must be indented as far as outer module declarations to indicate that they are inner modules, not new modules. For example, compare the following two examples. Module **Z** is an inner module in the following code.

[!CODE [FsModules#6607](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules7.fs#6607)]
    But module **Z** is a sibling to module **Y** in the following code.

[!CODE [FsModules#6608](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules7.fs#6608)]
    Module **Z** is also a sibling module in the following code, because it is not indented as far as other declarations in module **Y**.

[!CODE [FsModules#6609](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules7.fs#6609)]
    Finally, if the outer module has no declarations and is followed immediately by another module declaration, the new module declaration is assumed to be an inner module, but the compiler will warn you if the second module definition is not indented farther than the first.

[!CODE [FsModules#6610](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules7.fs#6610)]
    To eliminate the warning, indent the inner module.

[!CODE [FsModules#6611](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules7.fs#6611)]
    If you want all the code in a file to be in a single outer module and you want inner modules, the outer module does not require the equal sign, and the declarations, including any inner module declarations, that will go in the outer module do not have to be indented. Declarations inside the inner module declarations do have to be indented. The following code shows this case.

[!CODE [FsModules#6612](../CodeSnippet/VS_Snippets_Fsharp/fsmodules/FSharp/fs/modules6.fs#6612)]
    
## See Also
[F&#35; Language Reference](F%23+Language+Reference.md)

[Namespaces &#40;F&#35;&#41;](Namespaces+28%F%2329%.md)

