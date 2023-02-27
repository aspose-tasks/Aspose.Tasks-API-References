---
title: Class License
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.License classe. Fornisce metodi per concedere in licenza il componente.
type: docs
weight: 860
url: /it/net/aspose.tasks/license/
---
## License class

Fornisce metodi per concedere in licenza il componente.

```csharp
public class License
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [License](license/)() | Inizializza una nuova istanza di`License` classe. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | Concede in licenza il componente. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | Concede in licenza il componente. |

### Esempi

In questo esempio, verrà effettuato un tentativo di trovare un file di licenza denominato MyLicense.lic nella cartella che contiene  il componente, nella cartella che contiene l'assembly chiamante, nella cartella dell'assembly di entrata e poi nelle risorse embedded dell'assembly chiamante.

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

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks/)
* assemblea [Aspose.Tasks](../../)


