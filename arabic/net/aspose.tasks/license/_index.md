---
title: "الفئة License"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.License. توفر طرقًا لترخيص المكوّن."
type: docs
weight: 980
url: /ar/net/aspose.tasks/license/
---
## License class

يوفر طرقًا لترخيص المكوّن.

```csharp
public sealed class License
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [License](license/)() | يُنشئ مثيلًا جديدًا للفئة `License`. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | يرخص المكوّن. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | يرخص المكوّن. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


