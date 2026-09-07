---
title: "Project.Project"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore di Project. Inizializza una nuova istanza della classe Project."
type: docs
weight: 10
url: /it/net/aspose.tasks/project/project/
---
## Project() {#constructor}

Inizializza una nuova istanza della classe [`Project`](../).

```csharp
public Project()
```

## Esempi

Mostra come creare un progetto e salvarlo in formato MPP senza fornire un file modello MPP.

```csharp
var project = new Project();

// Il progetto sarà salvato in MPP utilizzando un modello MPP interno.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

Inizializza una nuova istanza della classe [`Project`](../) da un modello protetto da password (file mpp o mpt esistente).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | Stringa | Percorso del modello da cui creare il progetto. |
| protectionPassword | Stringa | Password di protezione. |

## Osservazioni

La lettura di file protetti da password è attualmente supportata solo per il formato file MSP 2003.

## Esempi

Mostra come leggere file MPP protetti da password.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

Inizializza una nuova istanza della classe [`Project`](../) da un modello (file mpp o mpt esistente).

```csharp
public Project(string projectTemplate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | Stringa | Percorso del modello da cui creare il progetto. |

## Esempi

Mostra come leggere un file MPP.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

Inizializza una nuova istanza della classe [`Project`](../) dallo Stream con l'istanza specificata della classe [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Flusso della classe Project Streamclass |
| options | PrimaveraReadOptions | l'istanza specificata della classe [`PrimaveraReadOptions`](../../primaverareadoptions/) che consente di personalizzare la lettura dei formati Primavera (XER o XML). |

## Esempi

Mostra come leggere un progetto da un flusso con un file Primavera XML o Primavera XER contenente più progetti.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // Restituisce il progetto con UID speciale
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Vedi anche

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

Inizializza una nuova istanza della classe [`Project`](../) da un modello (file mpp o mpt esistente).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | Stringa | Percorso del modello da cui creare il progetto. |
| parseErrorHandler | ParseErrorCallback | il metodo di callback specificato per gestire gli errori di parsing XML. |

## Esempi

Mostra come leggere un progetto da uno stream con un file XML contenente caratteri non validi.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // apri il file che contiene XML con intervalli di tempo interrotti
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

### Vedi anche

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

Inizializza una nuova istanza della classe [`Project`](../) da un flusso.

```csharp
public Project(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Flusso da cui caricare un modello. |

## Esempi

Mostra come leggere un file di progetto XML da un flusso.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

Inizializza una nuova istanza della classe [`Project`](../) da un'istanza di StreamReader.

```csharp
public Project(StreamReader reader)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| reader | StreamReader | Il lettore di flusso da cui caricare un modello. |

## Esempi

Mostra come leggere file MPX con una codifica specifica.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

Inizializza una nuova istanza della classe [`Project`](../) da un modello (file MPP o MPT esistente) con l'istanza specificata della classe [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | Stringa | Percorso al modello da cui creare il progetto |
| options | PrimaveraReadOptions | l'istanza specificata della classe [`PrimaveraReadOptions`](../../primaverareadoptions/). |

## Esempi

Mostra come leggere un progetto da un file Primavera XML o Primavera XER contenente più progetti utilizzando le opzioni di lettura Primavera.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// Restituisce il progetto con UID speciale
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Vedi anche

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

Inizializza una nuova istanza della classe [`Project`](../) per leggere i dati da un database specificato dall'istanza della classe [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/).

```csharp
public Project(DbSettings settings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| settings | DbSettings | l'istanza specificata della classe [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/). |

## Esempi

Mostra come importare un progetto da un database Primavera utilizzando le impostazioni del database.

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

// Inizializza una nuova istanza della classe PrimaveraDbSettings con la stringa di connessione e l'ID del progetto
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Inizializza una nuova istanza della classe Project
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Vedi anche

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

Inizializza una nuova istanza della classe [`Project`](../) da un modello (file mpp o mpt esistente).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Flusso da cui caricare un modello. |
| parseErrorHandler | ParseErrorCallback | il metodo di callback specificato per gestire gli errori di parsing XML. |

## Esempi

Mostra come leggere un progetto da un file XML con caratteri non validi.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // apri lo stream che contiene XML con intervalli di tempo interrotti
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

### Vedi anche

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

Inizializza una nuova istanza della classe [`Project`](../) da un modello (file mpp o mpt esistente).

```csharp
public Project(Stream stream, string protectionPassword)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Flusso da cui caricare un modello. |
| protectionPassword | Stringa | Password di protezione. |

## Osservazioni

La lettura di file protetti da password è attualmente supportata solo per il formato file MSP 2003.

## Esempi

Mostra come verificare se MPP è protetto da password.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

Mostra come leggere file MPP protetti da password da uno stream.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

Inizializza una nuova istanza della classe [`Project`](../) da un modello (file mpp o mpt esistente) con l'istanza specificata della classe [`LoadOptions`](../../loadoptions/).

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectTemplate | Stringa | Percorso al modello da cui creare il progetto |
| options | LoadOptions | l'istanza specificata della classe [`LoadOptions`](../../loadoptions/). |

## Esempi

Mostra come caricare il progetto da un file usando l'istanza &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

Mostra come leggere un progetto da un file XML Primavera con errori di analisi.

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

// Restituisce il progetto con UID speciale
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### Vedi anche

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

Inizializza una nuova istanza della classe [`Project`](../) dallo Stream con l'istanza specificata della classe [`LoadOptions`](../../loadoptions/).

```csharp
public Project(Stream stream, LoadOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Flusso della classe Project Streamclass |
| options | LoadOptions | l'istanza specificata della classe [`LoadOptions`](../../loadoptions/) |

## Esempi

Mostra come caricare il progetto da uno stream usando l'istanza &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

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

### Vedi anche

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


