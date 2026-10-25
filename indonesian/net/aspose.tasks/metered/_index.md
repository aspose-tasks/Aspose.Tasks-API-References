---
title: "Kelas Metered"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Metered. Menyediakan metode untuk mengatur kunci metered"
type: docs
weight: 1020
url: /id/net/aspose.tasks/metered/
---
## Metered class

Menyediakan metode untuk mengatur kunci bermeter.

```csharp
public class Metered
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Metered](metered/)() | Konstruktor default. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | Memeriksa apakah produk berhasil dilisensikan menggunakan lisensi Metered. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Menghapus lisensi yang sebelumnya disiapkan. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Mengatur kunci publik dan privat metered. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Mendapatkan kredit konsumsi. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Mendapatkan ukuran file konsumsi. |

## Contoh

Dalam contoh ini, akan dilakukan percobaan untuk mengatur kunci publik dan privat metered.

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

file jar komponen:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

Menampilkan cara menggunakan &lt;see cref="Aspose.Tasks.Metered" /&gt; tipe lisensi dengan Aspose.Tasks.

```csharp
// Mari gunakan lisensi metered (lihat https://purchase.aspose.com/faqs/licensing/metered)
// atur lisensi metered
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// bekerja dengan proyek...
// ...

// Kita dapat memperoleh kredit saat ini dan konsumsi byte.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // catat pengecualian
}

// baru-baru ini pengguna dapat mereset metered dan menghentikan penghitungan byte
metered.ResetMeteredKey();
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


