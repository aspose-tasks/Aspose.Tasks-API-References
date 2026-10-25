---
title: "NullableBool.IsDefined"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti NullableBool. Mengembalikan nilai yang menunjukkan apakah nilai telah didefinisikan, jika tidak false."
type: docs
weight: 20
url: /id/net/aspose.tasks/nullablebool/isdefined/
---
## NullableBool.IsDefined property

Mendapatkan nilai yang menunjukkan apakah nilai tersebut didefinisikan; jika tidak, false.

```csharp
public bool IsDefined { get; }
```

## Contoh

Menampilkan cara bekerja dengan kelas &lt;see cref="NullableBool" /&gt;.

```csharp
var project = new Project();

// Mari periksa di mana kelas <see cref="Aspose.Tasks.NullableBool" /> digunakan
// keuntungan utama dari <see cref="Aspose.Tasks.NullableBool" /> adalah 
// seseorang dapat mengaturnya sebagai tidak terdefinisi melalui konstruktor
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// gunakan instance nullable bool
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// gunakan instance nullable bool
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### Lihat Juga

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


