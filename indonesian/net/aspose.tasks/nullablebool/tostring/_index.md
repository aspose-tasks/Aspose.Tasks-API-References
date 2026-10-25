---
title: "NullableBool.ToString"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode NullableBool. Mengembalikan string yang merepresentasikan objek saat ini."
type: docs
weight: 60
url: /id/net/aspose.tasks/nullablebool/tostring/
---
## NullableBool.ToString method

Mengembalikan string yang mewakili objek saat ini.

```csharp
public override string ToString()
```

### Nilai Kembali

String yang merepresentasikan objek saat ini.

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


