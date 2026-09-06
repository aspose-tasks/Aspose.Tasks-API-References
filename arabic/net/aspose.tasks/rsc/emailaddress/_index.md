---
title: "Rsc.EMailAddress"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. عنوان البريد الإلكتروني للمورد"
type: docs
weight: 280
url: /ar/net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

عنوان البريد الإلكتروني للمورد.

```csharp
public static readonly Key<string, RscKey> EMailAddress;
```

## الأمثلة

يعرض كيفية ضبط خصائص الميتا الخاصة بالمورد.

```csharp
var project = new Project(DataDir + "Project.mpp");

// أضف موردًا واضبط بيانات الميتا للمورد
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


