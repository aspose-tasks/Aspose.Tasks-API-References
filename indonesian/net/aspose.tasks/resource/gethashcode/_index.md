---
title: "Resource.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Resource. Mengembalikan nilai kode hash untuk instance kelas Resource"
type: docs
weight: 840
url: /id/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

Mengembalikan nilai kode hash untuk instance kelas [`Resource`](../).

```csharp
public override int GetHashCode()
```

### Nilai Kembali

mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari sumber daya.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// kode hash dari sumber daya sama dengan UID sumber daya 
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### Lihat Juga

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


