# MailboxProcessor.Post<'Msg> Method (F#)

Posts a message to the message queue of the [MailboxProcessor](http://msdn.microsoft.com/en-us/library/2052c977-f787-4a0b-b25f-9444e26b5fdf), asynchronously.

**Namespace/Module Path**: Microsoft.FSharp.Control

**Assembly**: FSharp.Core (in FSharp.Core.dll)


## [!INCLUDE[System_CAPS_syntax](//System/Token/System_CAPS_syntax_md.md)]

```
// Signature:
member this.Post : 'Msg -> unit

// Usage:
mailboxProcessor.Post (message)
```

#### [!INCLUDE[System_CAPS_parameters](//System/Token/System_CAPS_parameters_md.md)]
*message*
Type: **'Msg**


The message to post.




## [!INCLUDE[System_CAPS_remarks](//System/Token/System_CAPS_remarks_md.md)]
**The following code example shows how to start a mailbox processor agent and post messages to it.**
**[!CODE [FsMailboxProcessor#2](../CodeSnippet/VS_Snippets_Fsharp/fsmailboxprocessor/FSharp/fs/program.fs#2)]**
**Following is an example session.**
**Press any key...**
**Message count = 0. Waiting for next message.**
**Message received. ID: 1 Contents: ABC**
**Message count = 1. Waiting for next message.**
**Message received. ID: 2 Contents: XYZ**
**Message count = 2. Waiting for next message.**
## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Control.MailboxProcessor&#60;'Msg&#62; Class &#40;F&#35;&#41;](Control.MailboxProcessor%3C%27Msg%3E+Class+28%F%2329%.md)

[Microsoft.FSharp.Control Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Control+Namespace+28%F%2329%.md)

