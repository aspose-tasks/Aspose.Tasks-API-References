---
title: "Aspose::Tasks::License class"
linktitle: "License"
articleTitle: "License"
second_title: "Aspose.Tasks for C++"
description: "Provides methods to license the component."
type: docs
weight: 10
url: /cpp/aspose.tasks/license/
---

## License class

Provides methods to license the component.

In this example, an attempt will be made to find a license file named MyLicense.lic in the folder that contains <ms> the component, in the folder that contains the calling assembly, in the folder of the entry assembly and then in the embedded resources of the calling assembly.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> the component jar file:

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## Constructors

| Name | Description |
| --- | --- |
| [License](./license/) | Initializes a new instance of the License class. |

## Methods

| Name | Description |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | Licenses the component. |

