---
title: "Aspose::Tasks::License class"
linktitle: "رخصة"
articleTitle: "رخصة"
second_title: "Aspose.Tasks لـ C++"
description: "يوفر طرقًا لترخيص المكوّن."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/license/
---

## License class

يوفر طرقًا لترخيص المكوّن.

في هذا المثال، سيتم محاولة العثور على ملف ترخيص باسم MyLicense.lic في المجلد الذي يحتوي على <ms> المكوّن، وفي المجلد الذي يحتوي على التجميع المستدعي، في مجلد التجميع الرئيسي، ثم في الموارد المدمجة للتجميع المستدعي.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> ملف jar للمكوّن:

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [License](./license/) | يقوم بتهيئة نسخة جديدة من الفئة License. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | يرخص المكوّن. |

