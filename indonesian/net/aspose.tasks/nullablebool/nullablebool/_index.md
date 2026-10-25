---
title: "NullableBool.NullableBool"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor NullableBool. Menginisialisasi instance baru dari struct NullableBool dengan nilai boolean yang ditentukan."
type: docs
weight: 10
url: /id/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

Menginisialisasi instance baru dari struct [`NullableBool`](../) dengan nilai boolean yang ditentukan.

```csharp
public NullableBool(bool value)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | Boolean | nilai boolean yang ditentukan. |

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

---

## NullableBool(bool, bool) {#constructor_1}

Menginisialisasi instance baru dari struct [`NullableBool`](../).

```csharp
public NullableBool(bool value, bool isDefined)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | Boolean | Nilai saat ini. |
| isDefined | Boolean | Nilai yang menunjukkan apakah nilai saat ini didefinisikan. |

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


