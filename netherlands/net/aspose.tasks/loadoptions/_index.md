---
title: "Klasse LoadOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.LoadOptions klasse. Stelt toe om extra laadparameters op te geven bij het laden van een project vanuit een bestand of stream."
type: docs
weight: 990
url: /nl/net/aspose.tasks/loadoptions/
---
## LoadOptions class

Staat toe extra laadparameters op te geven bij het laden van een project vanuit een bestand of stream.

```csharp
public class LoadOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [LoadOptions](loadoptions/)() | Initialiseert een nieuw exemplaar van de `LoadOptions` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | Haalt een token op of stelt deze in die kan worden gebruikt om een projectlaadoperatie te annuleren. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | Haalt de codering op of stelt deze in die wordt gebruikt om een project te lezen uit HTML-, MPX-, XER- en Primavera XML-formaten. De standaardcodering is UTF8. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | Haalt een callback-methode op of stelt deze in om XML-parsefouten af te handelen. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | Haalt een beschermingswachtwoord op of stelt dit in. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | Haalt een opgegeven instantie van de [`PrimaveraReadOptions`](../primaverareadoptions/) klasse op of stelt deze in, die kan worden gebruikt om het gedrag van het laden van Primavera-formaten (Primavera P6 XER of Primavera P6 Xml) aan te passen. |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | Haalt de callback op of stelt deze in die wordt aangeroepen tijdens projectlaadoperaties. Momenteel ondersteund voor MPP- en XER-formaten. |

## Voorbeelden

Toont hoe een wachtwoordbeveiligd project te laden met een &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; instantie.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


