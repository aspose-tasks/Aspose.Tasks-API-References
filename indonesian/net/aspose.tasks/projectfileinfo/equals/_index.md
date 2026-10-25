---
title: "ProjectFileInfo.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "ProjectFileInfo metode. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan"
type: docs
weight: 50
url: /id/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public bool Equals(ProjectFileInfo other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lain | ProjectFileInfo | Objek yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

mengembalikan true jika ProjectFileInfo yang ditentukan dan instance ini memiliki format file serta informasi aplikasi yang sama.

## Contoh

Menampilkan cara membaca informasi file proyek.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Lihat Juga

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | Objek yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

mengembalikan true jika ProjectFileInfo yang ditentukan dan instance ini memiliki format file serta informasi aplikasi yang sama.

## Contoh

Menampilkan cara membaca informasi file proyek.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Lihat Juga

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


