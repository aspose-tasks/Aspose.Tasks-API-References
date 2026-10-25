---
title: "License.License"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ License. ينشئ مثيلًا جديدًا لفئة License"
type: docs
weight: 10
url: /ar/net/aspose.tasks/license/license/
---
## License constructor

ينشئ مثيلًا جديدًا لفئة [`License`](../).

```csharp
public License()
```

## الأمثلة

في هذا المثال، سيتم محاولة العثور على ملف ترخيص يُدعى MyLicense.lic في المجلد الذي يحتوي على المكوّن، وفي المجلد الذي يحتوي على التجميع المستدعي، وفي مجلد التجميع الرئيسي، ثم في الموارد المدمجة للتجميع المستدعي.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

ملف jar المكوّن:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

يوضح كيفية تطبيق ترخيص Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### انظر أيضًا

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


