---
title: Project.Project
second_title: Aspose.Tasks for .NET API Reference
description: Project constructor. Initializes a new instance of the Project class
type: docs
weight: 10
url: /net/aspose.tasks/project/project/
---
## Project() {#constructor}

Initializes a new instance of the [`Project`](../) class.

```csharp
public Project()
```

## Examples

Shows how to create a project and save it into MPP format without passing of an MPP template file.

```csharp
var project = new Project();

// The project will be saved into MPP by using internal MPP template.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

Initializes a new instance of the [`Project`](../) class from a password protected template (existent mpp or mpt file).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from. |
| protectionPassword | String | Protection password. |

## Remarks

Reading password protected files currently supported for MSP 2003 file format only.

## Examples

Shows how to read password protected MPP files.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

Initializes a new instance of the [`Project`](../) class from a template (existent mpp or mpt file).

```csharp
public Project(string projectTemplate)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from. |

## Examples

Shows how to read a MPP file.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

Initializes a new instance of the [`Project`](../) class from the Stream with the specified instance of the [`PrimaveraReadOptions`](../../primaverareadoptions/) class.

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream of the Project Streamclass |
| options | PrimaveraReadOptions | the specified instance of the [`PrimaveraReadOptions`](../../primaverareadoptions/)class which allows to customize reading of Primavera formats (XER or XML). |

## Examples

Shows how to read a project from a stream with Primavera XML or Primavera XER file containing multiple projects.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // Returns project with special Uid
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### See Also

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

Initializes a new instance of the [`Project`](../) class from a template (existent mpp or mpt file).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from. |
| parseErrorHandler | ParseErrorCallback | the specified callback method to handle xml parse errors. |

## Examples

Shows how to read a project from a stream with XML file with invalid characters.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // open the file which contains XML with broken timespans
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

### See Also

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

Initializes a new instance of the [`Project`](../) class from a stream.

```csharp
public Project(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream to load a template from. |

## Examples

Shows how to read XML project file from a stream.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

Initializes a new instance of the [`Project`](../) class from a StreamReader instance.

```csharp
public Project(StreamReader reader)
```

| Parameter | Type | Description |
| --- | --- | --- |
| reader | StreamReader | The stream reader where to load a template from. |

## Examples

Shows how to read MPX files with specific encoding.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

Initializes a new instance of the [`Project`](../) class from a template (existent MPP or MPT file) with the specified instance of the [`PrimaveraReadOptions`](../../primaverareadoptions/) class.

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from |
| options | PrimaveraReadOptions | the specified instance of the [`PrimaveraReadOptions`](../../primaverareadoptions/) class. |

## Examples

Shows how to read a project from a Primavera XML or Primavera XER file containing multiple projects by using Primavera reading options.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// Returns project with special Uid
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### See Also

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

Initializes a new instance of the [`Project`](../) class to read data from a database which is specified by the instance of the [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) class.

```csharp
public Project(DbSettings settings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| settings | DbSettings | the specified instance of the [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) class. |

## Examples

Shows how to import a project from a Primavera database by using database settings.

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

// Initialize a new instance of the PrimaveraDbSettings class with connection string and project id
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Initialize a new instance of the Project class
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### See Also

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

Initializes a new instance of the [`Project`](../) class from a template(existent mpp or mpt file).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream to load a template from. |
| parseErrorHandler | ParseErrorCallback | the specified callback method to handle xml parse errors. |

## Examples

Shows how to read a project from XML file with invalid characters.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // open the stream which contains XML with broken timespans
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

### See Also

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

Initializes a new instance of the [`Project`](../) class from a template(existent mpp or mpt file).

```csharp
public Project(Stream stream, string protectionPassword)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream to load a template from. |
| protectionPassword | String | Protection password. |

## Remarks

Reading password protected files currently supported for MSP 2003 file format only.

## Examples

Shows how to check if MPP is password protected.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

Shows how to read password protected MPP files from a stream.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

Initializes a new instance of the [`Project`](../) class from a template (existent mpp or mpt file) with the specified instance of the [`LoadOptions`](../../loadoptions/) class.

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from |
| options | LoadOptions | the specified instance of the [`LoadOptions`](../../loadoptions/) class. |

## Examples

Shows how to load the project from a file by using &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; instance.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

Shows how to read a project from a Primavera XML file with error parsing.

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

// Returns project with special Uid
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### See Also

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

Initializes a new instance of the [`Project`](../) class from the Stream with the specified instance of the [`LoadOptions`](../../loadoptions/) class.

```csharp
public Project(Stream stream, LoadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream of the Project Streamclass |
| options | LoadOptions | the specified instance of the [`LoadOptions`](../../loadoptions/)class |

## Examples

Shows how to load the project from a stream by using &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; instance.

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

### See Also

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


