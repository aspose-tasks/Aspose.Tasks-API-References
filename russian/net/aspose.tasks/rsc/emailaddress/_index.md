---
title: "Rsc.EMailAddress"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Адрес электронной почты ресурса"
type: docs
weight: 280
url: /ru/net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

Электронный адрес ресурса.

```csharp
public static readonly Key<string, RscKey> EMailAddress;
```

## Примеры

Показывает, как установить мета‑свойства ресурса.

```csharp
var project = new Project(DataDir + "Project.mpp");

// Добавить ресурс и установить метаданные ресурса
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


