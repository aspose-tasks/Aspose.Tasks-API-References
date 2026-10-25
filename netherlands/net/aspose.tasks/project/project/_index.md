---
title: "Project.Project"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-constructeur. Initialiseert een nieuwe instantie van de Project-klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks/project/project/
---
## Project() {#constructor}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse.

```csharp
public Project()
```

## Voorbeelden

Toont hoe een project te maken en op te slaan in MPP-formaat zonder een MPP-sjabloonbestand te gebruiken.

```csharp
var project = new Project();

// Het project wordt opgeslagen in MPP met behulp van een interne MPP-sjabloon.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse vanuit een met wachtwoord beschermd sjabloon (bestaand mpp- of mpt-bestand).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | String | Pad naar sjabloon om project van te maken. |
| protectionPassword | String | Beschermingswachtwoord. |

## Opmerkingen

Het lezen van met wachtwoord beschermde bestanden wordt momenteel alleen ondersteund voor het MSP 2003-bestandsformaat.

## Voorbeelden

Toont hoe met wachtwoord beschermde MPP-bestanden te lezen.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

```csharp
public Project(string projectTemplate)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | String | Pad naar sjabloon om project van te maken. |

## Voorbeelden

Toont hoe een MPP-bestand te lezen.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse vanuit de Stream met de opgegeven instantie van de [`PrimaveraReadOptions`](../../primaverareadoptions/) klasse.

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | Stroom van de Project Streamclass |
| options | PrimaveraReadOptions | de opgegeven instantie van de [`PrimaveraReadOptions`](../../primaverareadoptions/)klasse die het mogelijk maakt om het lezen van Primavera-formaten (XER of XML) aan te passen. |

## Voorbeelden

Toont hoe een project te lezen vanuit een stroom met een Primavera XML- of Primavera XER-bestand dat meerdere projecten bevat.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // Retourneert project met speciale UID
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Zie ook

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | String | Pad naar sjabloon om project van te maken. |
| parseErrorHandler | ParseErrorCallback | de opgegeven callback-methode om xml-parsefouten af te handelen. |

## Voorbeelden

Toont hoe een project te lezen vanuit een stream met een XML‑bestand met ongeldige tekens.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // open het bestand dat XML met gebroken tijdsintervallen bevat
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### Zie ook

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse vanuit een stroom.

```csharp
public Project(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | Stroom om een sjabloon vanuit te laden. |

## Voorbeelden

Toont hoe een XML-projectbestand te lezen vanuit een stroom.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse vanuit een StreamReader‑instantie.

```csharp
public Project(StreamReader reader)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| reader | StreamReader | De streamlezer waar een sjabloon vanuit te laden is. |

## Voorbeelden

Toont hoe MPX-bestanden te lezen met een specifieke codering.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse vanuit een sjabloon (bestaand MPP- of MPT-bestand) met de opgegeven instantie van de [`PrimaveraReadOptions`](../../primaverareadoptions/) klasse.

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | String | Pad naar sjabloon om project van te maken |
| options | PrimaveraReadOptions | de opgegeven instantie van de [`PrimaveraReadOptions`](../../primaverareadoptions/) klasse. |

## Voorbeelden

Toont hoe een project te lezen vanuit een Primavera XML- of Primavera XER-bestand dat meerdere projecten bevat door gebruik te maken van Primavera-leesopties.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// Retourneert project met speciale UID
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Zie ook

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse om gegevens te lezen uit een database die wordt gespecificeerd door de instantie van de [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) klasse.

```csharp
public Project(DbSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | DbSettings | de opgegeven instantie van de [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) klasse. |

## Voorbeelden

Toont hoe een project te importeren vanuit een Primavera-database door gebruik te maken van database‑instellingen.

```csharp
var sb = new SqlConnectionStringBuilder
{
    DataSource = "192.168.56.3,1433",
    Encrypt = true,
    TrustServerCertificate = true,
    InitialCatalog = "PrimaveraEDB",
    NetworkLibrary = "DBMSSOCN",
    UserID = "privuser",
    Password = "***",
};

// Initialiseer een nieuw exemplaar van de PrimaveraDbSettings klasse met verbindingsreeks en project-ID
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Initialiseer een nieuwe instantie van de Project‑klasse
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Zie ook

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | Stroom om een sjabloon vanuit te laden. |
| parseErrorHandler | ParseErrorCallback | de opgegeven callback-methode om xml-parsefouten af te handelen. |

## Voorbeelden

Toont hoe een project te lezen uit een XML‑bestand met ongeldige tekens.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // open de stream die XML met gebroken tijdsintervallen bevat
    byte[] bytes = Encoding.UTF8.GetBytes(brokenXmlData);
    using (var stream = new MemoryStream(bytes))
    {
        var project = new Project(stream, CustomDurationHandlerForStream2);
        Console.WriteLine(project.Get(Prj.Name));
    }
}

public static object CustomDurationHandlerForStream2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Debug.Print("Object field : {0}, Invalid value : {1}", args.FieldName, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Debug.Print("New value : {0}", newValue);
    return newValue;
}
```

### Zie ook

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

Initialiseert een nieuwe instantie van de [`Project`](../) klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

```csharp
public Project(Stream stream, string protectionPassword)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | Stroom om een sjabloon vanuit te laden. |
| protectionPassword | String | Beschermingswachtwoord. |

## Opmerkingen

Het lezen van met wachtwoord beschermde bestanden wordt momenteel alleen ondersteund voor het MSP 2003-bestandsformaat.

## Voorbeelden

Toont hoe te controleren of MPP met een wachtwoord is beveiligd.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

Toont hoe wachtwoordbeveiligde MPP‑bestanden uit een stream te lezen.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

Initialiseert een nieuwe instantie van de [`Project`](../)‑klasse vanuit een sjabloon (bestaand mpp‑ of mpt‑bestand) met de opgegeven instantie van de [`LoadOptions`](../../loadoptions/)‑klasse.

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectTemplate | String | Pad naar sjabloon om project van te maken |
| options | LoadOptions | de opgegeven instantie van de [`LoadOptions`](../../loadoptions/)‑klasse. |

## Voorbeelden

Toont hoe het project te laden vanuit een bestand met behulp van een &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;‑instantie.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

Toont hoe een project te lezen uit een Primavera‑XML‑bestand met fouten bij het parseren.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// Retourneert project met speciale UID
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### Zie ook

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

Initialiseert een nieuwe instantie van de [`Project`](../)‑klasse vanuit de Stream met de opgegeven instantie van de [`LoadOptions`](../../loadoptions/)‑klasse.

```csharp
public Project(Stream stream, LoadOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | Stroom van de Project Streamclass |
| options | LoadOptions | de opgegeven instantie van de [`LoadOptions`](../../loadoptions/)klasse |

## Voorbeelden

Toont hoe het project te laden vanuit een stream met behulp van een &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;‑instantie.

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

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


