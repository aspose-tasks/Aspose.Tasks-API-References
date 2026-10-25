---
title: "Project.Save"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-methode. Slaat het document op in een bestand met behulp van de opgegeven opslagopties."
type: docs
weight: 1200
url: /nl/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

Slaat het document op in een bestand met behulp van de opgegeven opslagopties.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestandsnaam | String | De bestandsnaam. |
| opties | SimpleSaveOptions | De opslagopties. |

## Voorbeelden

Toont hoe een project op te slaan als een MPP-bestand.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### Zie ook

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

Slaat de projectgegevens op in het bestand.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestandsnaam | String | De bestandsnaam. |
| formaat | SaveFileFormat | Het opslagbestandsformaat. |

## Voorbeelden

Toont hoe een project te maken en op te slaan in MPP-formaat zonder een MPP-sjabloonbestand te gebruiken.

```csharp
var project = new Project();

// Het project wordt opgeslagen in MPP met behulp van een interne MPP-sjabloon.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

Slaat de projectgegevens op in het bestand in mpp-indeling.

```csharp
public void Save(string filename)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestandsnaam | String | De bestandsnaam. |

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

Slaat het project op in een stream met behulp van de opgegeven opslagopties.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | De stream. |
| opties | SimpleSaveOptions | De opslagopties. |

## Voorbeelden

Toont hoe een project in een stream op te slaan als een MPP-bestand met behulp van MPP-opslagopties.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // Door gebruik te maken van MPPSaveOptions slaan we het op in MPP-formaat.
    project.Save(stream, options);
}
```

Toont hoe een project in een stream op te slaan als een afbeelding en de afbeeldingopties te beheren.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // door gebruik te maken van ImageSaveOptions slaan we het project op in een afbeeldingsformaat
    project.Save(stream, options);
}
```

### Zie ook

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

Slaat de projectgegevens op in de stream.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | De stream. |
| format | SaveFileFormat | het opgegeven opslagbestandsformaat.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## Voorbeelden

Toont hoe een project in een stream op te slaan als een XML MS Project-bestand.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // Schrijf de stream in XML-formaat
    project.Save(stream, SaveFileFormat.Xml);
}
```

### Zie ook

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


