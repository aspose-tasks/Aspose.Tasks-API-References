---
title: "License.License"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore License. Inizializza una nuova istanza della classe License"
type: docs
weight: 10
url: /it/net/aspose.tasks/license/license/
---
## License constructor

Inizializza una nuova istanza della classe [`License`](../).

```csharp
public License()
```

## Esempi

In questo esempio, verrà tentato di trovare un file di licenza chiamato MyLicense.lic nella cartella che contiene il componente, nella cartella che contiene l'assembly chiamante, nella cartella dell'assembly di ingresso e poi nelle risorse incorporate dell'assembly chiamante.

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

Mostra come applicare una licenza di Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Vedi anche

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


