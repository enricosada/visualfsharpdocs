# QueryBuilder.MinByNullable<'T,'Q,'Value> Method (F#)

A query operator that selects a nullable value for each element selected so far and returns the minimum of these values. If any nullable does not have a value, it is ignored.

**Namespace/Module Path**: Microsoft.FSharp.Linq

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
member this.MinByNullable : QuerySource<'T,'Q> * ('T -> Nullable<'Value>) -> Nullable<'Value> when 'Value : (IComparable) and 'Value : (new : unit ->  'Value) and 'Value : struct and 'Value :> ValueType

// Usage:
queryBuilder.MinByNullable (source, valueSelector)
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*source*
Type: [QuerySource](http://msdn.microsoft.com/en-us/library/873589c1-c5dc-47d9-8abf-fee7258dfb00)&lt;'T,'Q&gt;


The input query.


*valueSelector*
Type: 'T -&gt;
**T:System.Nullable&#96;1**&lt;'Value&gt;


A function that computes the values to compare.




## Return Value
The minimum value, or the default value for the type.


## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
For more information and examples, see [Query Expressions (F#)](http://msdn.microsoft.com/en-us/library/ff72235c-3ad8-4215-8679-2754484823db).


## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 4.0, Portable




## See Also
[Linq.QueryBuilder Class &#40;F&#35;&#41;](Linq.QueryBuilder+Class+28%F%2329%.md)

[Microsoft.FSharp.Linq Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Linq+Namespace+28%F%2329%.md)

[Query Expressions (F#)](http://msdn.microsoft.com/en-us/library/ff72235c-3ad8-4215-8679-2754484823db)

