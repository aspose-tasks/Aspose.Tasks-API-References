---
title: "NullableBool.op_Implicit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode NullableBool. Secara implisit mengonversi instance NullableBool menjadi nilai boolean. Mengembalikan true ketika Value true dan IsDefined true."
type: docs
weight: 80
url: /id/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

Secara implisit mengonversi sebuah instance [`NullableBool`](../) menjadi nilai boolean. Mengembalikan true ketika [`Value`](../value/) true dan [`IsDefined`](../isdefined/) true.

```csharp
public static implicit operator bool(NullableBool val)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| val | NullableBool | Nilai yang akan dikonversi. |

### Nilai Kembali

sebuah nilai boolean.

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

---

## implicit operator {#op_implicit}

Secara implisit mengonversi nilai boolean menjadi instance [`NullableBool`](../).

```csharp
public static implicit operator NullableBool(bool val)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| val | Boolean | Nilai untuk dikonversi. |

### Nilai Kembali

Instance [`NullableBool`](../) yang dikonversi.

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


