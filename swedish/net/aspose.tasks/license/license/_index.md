---
title: License.License
second_title: Aspose.Tasks för .NET API-referens
description: License byggare. Initierar en ny instans avLicense klass.
type: docs
weight: 10
url: /sv/net/aspose.tasks/license/license/
---
## License constructor

Initierar en ny instans av[`License`](../) klass.

```csharp
public License()
```

### Exempel

I det här exemplet kommer ett försök att göras att hitta en licensfil med namnet MyLicense.lic i mappen som innehåller  komponenten, i mappen som innehåller den anropande sammansättningen, i mappen för postsammansättningen och sedan i de inbäddade resurserna för den anropande sammansättningen.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

komponentjarfilen:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Se även

* class [License](../)
* namnutrymme [Aspose.Tasks](../../license/)
* hopsättning [Aspose.Tasks](../../../)


