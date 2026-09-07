---
title: "Rsc.WindowsUserAccount"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Akun NT yang terkait dengan sumber daya"
type: docs
weight: 680
url: /id/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

Akun NT yang terkait dengan sebuah sumber daya.

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
```

## Contoh

Menampilkan cara mengatur properti meta sumber daya.

```csharp
var project = new Project(DataDir + "Project.mpp");

// Tambahkan sumber daya dan atur metadata sumber daya
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


