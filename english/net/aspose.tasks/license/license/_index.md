---
title: License.License
second_title: Aspose.Tasks for .NET API Reference
description: License constructor. Initializes a new instance of the License class
type: docs
weight: 10
url: /net/aspose.tasks/license/license/
---
## License constructor

Initializes a new instance of the [`License`](../) class.

```csharp
public License()
```

## Examples

In this example, an attempt will be made to find a license file named MyLicense.lic in the folder that contains  the component, in the folder that contains the calling assembly, in the folder of the entry assembly and then in the embedded resources of the calling assembly.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

the component jar file:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Shows how to apply a license of Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### See Also

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


