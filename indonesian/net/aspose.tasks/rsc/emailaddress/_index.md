---
title: "Rsc.EMailAddress"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Alamat email sebuah sumber daya"
type: docs
weight: 280
url: /id/net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

Alamat email sumber daya.

```csharp
public static readonly Key<string, RscKey> EMailAddress;
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


