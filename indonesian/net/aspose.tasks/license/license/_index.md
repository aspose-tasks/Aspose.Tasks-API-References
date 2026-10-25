---
title: "License.License"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor License. Menginisialisasi sebuah instance baru dari kelas License"
type: docs
weight: 10
url: /id/net/aspose.tasks/license/license/
---
## License constructor

Menginisialisasi sebuah instance baru dari kelas [`License`](../).

```csharp
public License()
```

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

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


