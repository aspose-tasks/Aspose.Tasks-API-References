---
title: "VbaReference.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode VbaReference. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek VbaReference yang ditentukan"
type: docs
weight: 40
url: /id/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek [`VbaReference`](../) yang ditentukan.

```csharp
public bool Equals(VbaReference other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | VbaReference | Objek [`VbaReference`](../) yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

Mengembalikan true jika instance ini sama dengan objek [`VbaReference`](../) yang ditentukan; jika tidak, false.

## Contoh

Menampilkan cara memeriksa kesetaraan referensi VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Kesetaraan referensi diperiksa berdasarkan nama referensi.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Lihat Juga

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek [`VbaReference`](../) yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Object | Objek [`VbaReference`](../) yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

Mengembalikan true jika instance ini sama dengan objek [`VbaReference`](../) yang ditentukan; jika tidak, false.

## Contoh

Menampilkan cara memeriksa kesetaraan referensi VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Kesetaraan referensi diperiksa berdasarkan nama referensi.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Lihat Juga

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


