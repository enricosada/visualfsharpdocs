# Patterns.LetRecursive Active Pattern (F#)

Recognizes expressions that represent recursive **let** bindings of one or more variables.

**Namespace/Module Path**: Microsoft.FSharp.Quotations.Patterns

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
( |LetRecursive|_| ) : (input:Expr) -> ((Var * Expr) list * Expr) option
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*input*
Type: [Expr](http://msdn.microsoft.com/en-us/library/ed6a2caf-69d4-45c2-ab97-e9b3be9bce65)


The input expression to match against.



**The formal return type is ((Var &#42; Expr) list &#42; Expr) option. The option indicates whether the input results in a match. In a pattern matching expression, the input is decomposed, upon a successful match, into a tuple that contains two elements. The first element is a list of tuples that has two elements. The first element of the inner tuple is a [Var](http://msdn.microsoft.com/en-us/library/2b1237f9-d897-4bcf-872a-4a297db3f7b5) object that represents the value being defined. The second element of the inner tuple represents the body of a recursive let binding. The second element of the outer tuple is the subexpression in which the binding is in scope.**
## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
This function is named **LetRecursivePattern** in the .NET Framework assembly. If you are accessing the member from a .NET Framework language other than F#, or through reflection, use this name.


## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Quotations.Patterns Module &#40;F&#35;&#41;](Quotations.Patterns+Module+28%F%2329%.md)

[Microsoft.FSharp.Quotations Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Quotations+Namespace+28%F%2329%.md)

