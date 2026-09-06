---
title: "Project.Project"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur du projet. Initialise une nouvelle instance de la classe Project."
type: docs
weight: 10
url: /fr/net/aspose.tasks/project/project/
---
## Project() {#constructor}

Initialise une nouvelle instance de la classe [`Project`](../).

```csharp
public Project()
```

## Exemples

Montre comment créer un projet et l'enregistrer au format MPP sans fournir de fichier de modèle MPP.

```csharp
var project = new Project();

// Le projet sera enregistré au format MPP en utilisant le modèle MPP interne.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

Initialise une nouvelle instance de la classe [`Project`](../) à partir d'un modèle protégé par mot de passe (fichier mpp ou mpt existant).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | Chaîne | Chemin vers le modèle à partir duquel créer le projet. |
| protectionPassword | Chaîne | Mot de passe de protection. |

## Remarques

La lecture de fichiers protégés par mot de passe est actuellement prise en charge uniquement pour le format de fichier MSP 2003.

## Exemples

Montre comment lire des fichiers MPP protégés par mot de passe.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

Initialise une nouvelle instance de la classe [`Project`](../) à partir d'un modèle (fichier mpp ou mpt existant).

```csharp
public Project(string projectTemplate)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | Chaîne | Chemin vers le modèle à partir duquel créer le projet. |

## Exemples

Montre comment lire un fichier MPP.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

Initialise une nouvelle instance de la classe [`Project`](../) à partir du flux avec l'instance spécifiée de la classe [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Flux du Project Streamclass |
| options | PrimaveraReadOptions | l'instance spécifiée de la classe [`PrimaveraReadOptions`](../../primaverareadoptions/) qui permet de personnaliser la lecture des formats Primavera (XER ou XML). |

## Exemples

Montre comment lire un projet à partir d'un flux avec un fichier Primavera XML ou Primavera XER contenant plusieurs projets.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // Renvoie le projet avec un UID spécial
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Voir aussi

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

Initialise une nouvelle instance de la classe [`Project`](../) à partir d'un modèle (fichier mpp ou mpt existant).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | Chaîne | Chemin vers le modèle à partir duquel créer le projet. |
| parseErrorHandler | ParseErrorCallback | la méthode de rappel spécifiée pour gérer les erreurs d'analyse XML. |

## Exemples

Montre comment lire un projet à partir d'un flux avec un fichier XML contenant des caractères invalides.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // ouvrir le fichier qui contient du XML avec des intervalles de temps corrompus
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

### Voir aussi

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

Initialise une nouvelle instance de la classe [`Project`](../) à partir d'un flux.

```csharp
public Project(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Flux à partir duquel charger un modèle. |

## Exemples

Montre comment lire un fichier de projet XML à partir d'un flux.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

Initialise une nouvelle instance de la classe [`Project`](../) à partir d'une instance de StreamReader.

```csharp
public Project(StreamReader reader)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| lecteur | StreamReader | Le lecteur de flux à partir duquel charger un modèle. |

## Exemples

Montre comment lire des fichiers MPX avec un encodage spécifique.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

Initialise une nouvelle instance de la classe [`Project`](../) à partir d'un modèle (fichier MPP ou MPT existant) avec l'instance spécifiée de la classe [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | Chaîne | Chemin vers le modèle à partir duquel créer le projet |
| options | PrimaveraReadOptions | l'instance spécifiée de la classe [`PrimaveraReadOptions`](../../primaverareadoptions/). |

## Exemples

Montre comment lire un projet à partir d'un fichier Primavera XML ou Primavera XER contenant plusieurs projets en utilisant les options de lecture Primavera.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// Renvoie le projet avec un UID spécial
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Voir aussi

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

Initialise une nouvelle instance de la classe [`Project`](../) pour lire des données depuis une base de données spécifiée par l'instance de la classe [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/).

```csharp
public Project(DbSettings settings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| settings | DbSettings | l'instance spécifiée de la classe [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/). |

## Exemples

Montre comment importer un projet depuis une base de données Primavera en utilisant les paramètres de la base de données.

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

// Initialiser une nouvelle instance de la classe PrimaveraDbSettings avec la chaîne de connexion et l'identifiant du projet
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Initialiser une nouvelle instance de la classe Project
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Voir aussi

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

Initialise une nouvelle instance de la classe [`Project`](../) à partir d'un modèle (fichier MPP ou MPT existant).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Flux à partir duquel charger un modèle. |
| parseErrorHandler | ParseErrorCallback | la méthode de rappel spécifiée pour gérer les erreurs d'analyse XML. |

## Exemples

Montre comment lire un projet à partir d'un fichier XML contenant des caractères invalides.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // ouvrir le flux qui contient du XML avec des intervalles de temps corrompus
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

### Voir aussi

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

Initialise une nouvelle instance de la classe [`Project`](../) à partir d'un modèle (fichier MPP ou MPT existant).

```csharp
public Project(Stream stream, string protectionPassword)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Flux à partir duquel charger un modèle. |
| protectionPassword | Chaîne | Mot de passe de protection. |

## Remarques

La lecture de fichiers protégés par mot de passe est actuellement prise en charge uniquement pour le format de fichier MSP 2003.

## Exemples

Montre comment vérifier si le MPP est protégé par mot de passe.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

Montre comment lire des fichiers MPP protégés par mot de passe depuis un flux.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

Initialise une nouvelle instance de la classe [`Project`](../) à partir d'un modèle (fichier mpp ou mpt existant) avec l'instance spécifiée de la classe [`LoadOptions`](../../loadoptions/).

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | Chaîne | Chemin vers le modèle à partir duquel créer le projet |
| options | LoadOptions | l'instance spécifiée de la classe [`LoadOptions`](../../loadoptions/). |

## Exemples

Montre comment charger le projet depuis un fichier en utilisant l'instance &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

Montre comment lire un projet à partir d'un fichier XML Primavera avec une erreur d'analyse.

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

// Renvoie le projet avec un UID spécial
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### Voir aussi

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

Initialise une nouvelle instance de la classe [`Project`](../) à partir du flux avec l'instance spécifiée de la classe [`LoadOptions`](../../loadoptions/).

```csharp
public Project(Stream stream, LoadOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Flux du Project Streamclass |
| options | LoadOptions | l'instance spécifiée de la classe [`LoadOptions`](../../loadoptions/)classe |

## Exemples

Montre comment charger le projet depuis un flux en utilisant l'instance &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

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

### Voir aussi

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


