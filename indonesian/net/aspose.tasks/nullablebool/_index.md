---
title: "Struct NullableBool"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.NullableBool struct. Kelas untuk nilai boolean dengan kemungkinan memeriksa apakah nilai tersebut telah didefinisikan atau tidak."
type: docs
weight: 1110
url: /id/net/aspose.tasks/nullablebool/
---
## NullableBool structure

Sebuah kelas untuk nilai boolean dengan kemampuan memeriksa apakah nilai tersebut telah didefinisikan atau tidak.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | Menginisialisasi instance baru dari struct `NullableBool` dengan nilai boolean yang ditentukan. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | Menginisialisasi instance baru dari struct `NullableBool`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | Mendapatkan nilai yang menunjukkan apakah nilai tersebut didefinisikan; jika tidak, false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah nilai saat ini true atau false. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | Mengembalikan flag yang menunjukkan apakah instance ini sama dengan instance yang ditentukan dari kelas `NullableBool`. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | Mengembalikan flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | Mengembalikan nilai kode hash untuk instance kelas `NullableBool`. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | Mengembalikan string yang mewakili objek saat ini. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | Secara implisit mengonversi instance `NullableBool` menjadi nilai boolean. Mengembalikan true ketika [`Value`](./value/) bernilai true dan [`IsDefined`](./isdefined/) bernilai true. (2 operator) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | Kembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


