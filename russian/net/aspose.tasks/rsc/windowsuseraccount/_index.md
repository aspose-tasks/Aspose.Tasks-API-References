---
title: "Rsc.WindowsUserAccount"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. NT‑учетная запись, связанная с ресурсом"
type: docs
weight: 680
url: /ru/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

Учётная запись NT, связанная с ресурсом.

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
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


