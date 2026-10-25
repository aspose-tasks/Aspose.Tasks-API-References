---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode PrimaveraBaseReader. Mengembalikan daftar identifier unik proyek"
type: docs
weight: 20
url: /id/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

Kembalikan daftar pengidentifikasi unik proyek.

```csharp
public List<int> GetProjectUids()
```

### Nilai Kembali

Daftar pengidentifikasi unik proyek.

## Contoh

Menampilkan cara mengimpor proyek dari file XML Primavera.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### Lihat Juga

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


