# NullableOperators.( ?>=? )<'T> Function (F#)

The **&gt;=** operator where a nullable value appears on both left and right sides.

**Namespace/Module Path**: Microsoft.FSharp.Linq.NullableOperators

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
( ?>=? ) : Nullable<'T> -> Nullable<'T> -> bool when 'T : (IComparable) and 'T : (new : unit ->  'T) and 'T : struct and 'T :> ValueType

// Usage:
nullableValue1 ?>=? nullableValue2
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*nullableValue1*
Type: **T:System.Nullable&#96;1**&lt;'T&gt;


The first input value, as a nullable value.


*nullableValue2*
Type: **T:System.Nullable&#96;1**&lt;'T&gt;


The second input value, as a nullable value.




## Return Value
**true** if the first input value is greater than or equal to the second.


## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
If either of the input values is null, then the result is **false**.


## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 4.0, Portable




## See Also
[Linq.NullableOperators Module &#40;F&#35;&#41;](Linq.NullableOperators+Module+28%F%2329%.md)

[Microsoft.FSharp.Linq Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Linq+Namespace+28%F%2329%.md)

