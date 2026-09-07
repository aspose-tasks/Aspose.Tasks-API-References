---
title: "VbaModuleAttribute.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode VbaModuleAttribute. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek VbaModuleAttribute yang ditentukan"
type: docs
weight: 30
url: /id/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek [`VbaModuleAttribute`](../) yang ditentukan.

```csharp
public bool Equals(VbaModuleAttribute other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | VbaModuleAttribute | Objek [`VbaModuleAttribute`](../) yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

Mengembalikan true jika instance ini sama dengan objek [`VbaModuleAttribute`](../) yang ditentukan; jika tidak, false.

## Contoh

Menampilkan cara memeriksa kesamaan atribut modul VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Lihat Juga

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek [`VbaModuleAttribute`](../) yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Object | Objek [`VbaModuleAttribute`](../) yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

Mengembalikan true jika instance ini sama dengan objek [`VbaModuleAttribute`](../) yang ditentukan; jika tidak, false.

## Contoh

Menampilkan cara memeriksa kesamaan atribut modul VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Lihat Juga

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


