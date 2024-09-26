---
title: Prj.MicrosoftProjectServerURL
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether a project was created by a Project Server user as opposed to an NT user
type: docs
weight: 460
url: /net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

Determines whether a project was created by a Project Server user as opposed to an NT user.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## Examples

Shows how to read/write Prj.MicrosoftProjectServerURL property.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


