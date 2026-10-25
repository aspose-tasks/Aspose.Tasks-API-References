---
title: "Kelas License"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.License. Menyediakan metode untuk melisensikan komponen"
type: docs
weight: 980
url: /id/net/aspose.tasks/license/
---
## License class

Menyediakan metode untuk melisensikan komponen.

```csharp
public sealed class License
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [License](license/)() | Menginisialisasi instance baru dari kelas `License`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | Melisensikan komponen. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | Melisensikan komponen. |

## Contoh

Dalam contoh ini, akan dilakukan upaya untuk menemukan file lisensi bernama MyLicense.lic di folder yang berisi komponen, di folder yang berisi assembly pemanggil, di folder assembly entri, dan kemudian di sumber daya tersemat dari assembly pemanggil.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

file jar komponen:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Menampilkan cara menerapkan lisensi Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


