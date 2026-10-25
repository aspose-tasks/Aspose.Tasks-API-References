---
title: "NullableBool.op_Equality"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode NullableBool. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan."
type: docs
weight: 70
url: /id/net/aspose.tasks/nullablebool/op_equality/
---
## NullableBool Equality operator

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public static bool operator ==(NullableBool a, NullableBool b)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | NullableBool | [`NullableBool`](../) pertama. |
| b | NullableBool | [`NullableBool`](../) kedua. |

### Nilai Kembali

nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan

## Contoh

Menampilkan cara membandingkan &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt; instance.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// Kesetaraan bool diperiksa terhadap properti 'IsDefined' dan 'Value'.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// memeriksa konversi implisit ke bool: bool1 adalah True karena didefinisikan dan Value diatur ke True.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// memeriksa konversi implisit ke bool: bool2 adalah False karena tidak didefinisikan.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// memeriksa konversi implisit ke bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### Lihat Juga

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


