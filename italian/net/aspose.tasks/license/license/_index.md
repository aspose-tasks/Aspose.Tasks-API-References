---
title: License
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Inizializza una nuova istanza diLicenseaspose.tasks/license classe.
type: docs
weight: 10
url: /it/net/aspose.tasks/license/license/
---
## License constructor

Inizializza una nuova istanza di[`License`](../../license) classe.

```csharp
public License()
```

### Esempi

In questo esempio, verrà effettuato un tentativo di trovare un file di licenza denominato MyLicense.lic nella cartella che contiene  il componente, nella cartella che contiene l'assembly chiamante, nella cartella dell'assembly di ingresso e quindi nelle risorse incorporate dell'assembly chiamante.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

il file jar del componente:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Guarda anche

* class [License](../../license)
* spazio dei nomi [Aspose.Tasks](../../license)
* assemblea [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->