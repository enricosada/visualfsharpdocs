# Members (F#)

This section describes members of F# object types.


## Remarks
*Members* are features that are part of a type definition and are declared with the **member** keyword. F# object types such as records, classes, discriminated unions, interfaces, and structures support members. For more information, see [Records &#40;F&#35;&#41;](Records+28%F%2329%.md), [Classes &#40;F&#35;&#41;](Classes+28%F%2329%.md), [Discriminated Unions &#40;F&#35;&#41;](Discriminated+Unions+28%F%2329%.md), [Interfaces &#40;F&#35;&#41;](Interfaces+28%F%2329%.md), and [Structures &#40;F&#35;&#41;](Structures+28%F%2329%.md).

Members typically make up the public interface for a type, which is why they are public unless otherwise specified. Members can also be declared private or internal. For more information, see [Access Control &#40;F&#35;&#41;](Access+Control+28%F%2329%.md). Signatures for types can also be used to expose or not expose certain members of a type. For more information, see [Signatures &#40;F&#35;&#41;](Signatures+28%F%2329%.md).

Private fields and **do** bindings, which are used only with classes, are not true members, because they are never part of the public interface of a type and are not declared with the **member** keyword, but they are described in this section also.


## Related Topics


|Topic|Description|
|-----|-----------|
|[let Bindings in Classes &#40;F&#35;&#41;](let+Bindings+in+Classes+28%F%2329%.md)|Describes the definition of private fields and functions in classes.|
|[do Bindings in Classes &#40;F&#35;&#41;](do+Bindings+in+Classes+28%F%2329%.md)|Describes the specification of object initialization code.|
|[Properties &#40;F&#35;&#41;](Properties+28%F%2329%.md)|Describes property members in classes and other types.|
|[Indexed Properties &#40;F&#35;&#41;](Indexed+Properties+28%F%2329%.md)|Describes array-like properties in classes and other types.|
|[Methods &#40;F&#35;&#41;](Methods+28%F%2329%.md)|Describes functions that are members of a type.|
|[Constructors &#40;F&#35;&#41;](Constructors+28%F%2329%.md)|Describes special functions that initialize objects of a type.|
|[Operator Overloading &#40;F&#35;&#41;](Operator+Overloading+28%F%2329%.md)|Describes the definition of customized operators for types.|
|[Events &#40;F&#35;&#41;](Events+28%F%2329%.md)|Describes the definition of events and event handling support in F#.|
|[Explicit Fields: The val Keyword &#40;F&#35;&#41;](Explicit+Fields%3A+The+val+Keyword+28%F%2329%.md)|Describes the definition of uninitialized fields in a type.|
