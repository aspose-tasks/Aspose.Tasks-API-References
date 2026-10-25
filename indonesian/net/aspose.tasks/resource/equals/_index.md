---
title: "Resource.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Resource. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan instance tertentu dari kelas Resource"
type: docs
weight: 820
url: /id/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan instance tertentu dari kelas [`Resource`](../).

```csharp
public bool Equals(Resource other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | Resource | Instance tertentu dari kelas [`Resource`](../) untuk dibandingkan dengan instance ini. |

### Nilai Kembali

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## Contoh

Menampilkan cara memeriksa kesetaraan sumber daya.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Lihat Juga

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | Objek untuk dibandingkan dengan instance ini. |

### Nilai Kembali

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## Contoh

Menampilkan cara memeriksa kesetaraan sumber daya.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Lihat Juga

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


