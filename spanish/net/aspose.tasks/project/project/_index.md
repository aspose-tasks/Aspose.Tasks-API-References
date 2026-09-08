---
title: "Project.Project"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de Project. Inicializa una nueva instancia de la clase Project."
type: docs
weight: 10
url: /es/net/aspose.tasks/project/project/
---
## Project() {#constructor}

Inicializa una nueva instancia de la clase [`Project`](../).

```csharp
public Project()
```

## Ejemplos

Muestra cómo crear un proyecto y guardarlo en formato MPP sin pasar un archivo de plantilla MPP.

```csharp
var project = new Project();

// El proyecto se guardará en MPP utilizando una plantilla MPP interna.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

Inicializa una nueva instancia de la clase [`Project`](../) a partir de una plantilla protegida con contraseña (archivo mpp o mpt existente).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | Cadena | Ruta a la plantilla desde la cual crear el proyecto. |
| protectionPassword | Cadena | Contraseña de protección. |

## Observaciones

La lectura de archivos protegidos con contraseña actualmente solo es compatible con el formato de archivo MSP 2003.

## Ejemplos

Muestra cómo leer archivos MPP protegidos con contraseña.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

Inicializa una nueva instancia de la clase [`Project`](../) a partir de una plantilla (archivo mpp o mpt existente).

```csharp
public Project(string projectTemplate)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | Cadena | Ruta a la plantilla desde la cual crear el proyecto. |

## Ejemplos

Muestra cómo leer un archivo MPP.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

Inicializa una nueva instancia de la clase [`Project`](../) a partir del Stream con la instancia especificada de la clase [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | Flujo del Project Streamclass |
| options | PrimaveraReadOptions | la instancia especificada de la clase [`PrimaveraReadOptions`](../../primaverareadoptions/) que permite personalizar la lectura de los formatos Primavera (XER o XML). |

## Ejemplos

Muestra cómo leer un proyecto desde un flujo con un archivo Primavera XML o Primavera XER que contiene varios proyectos.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // Devuelve el proyecto con UID especial.
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Ver también

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

Inicializa una nueva instancia de la clase [`Project`](../) a partir de una plantilla (archivo mpp o mpt existente).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | Cadena | Ruta a la plantilla desde la cual crear el proyecto. |
| parseErrorHandler | ParseErrorCallback | el método de devolución de llamada especificado para manejar errores de análisis XML. |

## Ejemplos

Muestra cómo leer un proyecto desde un flujo con un archivo XML con caracteres no válidos.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // abre el archivo que contiene XML con intervalos de tiempo rotos
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

### Ver también

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

Inicializa una nueva instancia de la clase [`Project`](../) a partir de un flujo.

```csharp
public Project(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | Flujo desde el cual cargar una plantilla. |

## Ejemplos

Muestra cómo leer un archivo de proyecto XML desde un flujo.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

Inicializa una nueva instancia de la clase [`Project`](../) a partir de una instancia de StreamReader.

```csharp
public Project(StreamReader reader)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lector | StreamReader | El lector de flujo desde el cual cargar una plantilla. |

## Ejemplos

Muestra cómo leer archivos MPX con una codificación específica.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

Inicializa una nueva instancia de la clase [`Project`](../) a partir de una plantilla (archivo MPP o MPT existente) con la instancia especificada de la clase [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | Cadena | Ruta a la plantilla desde la cual crear el proyecto |
| options | PrimaveraReadOptions | la instancia especificada de la clase [`PrimaveraReadOptions`](../../primaverareadoptions/). |

## Ejemplos

Muestra cómo leer un proyecto desde un archivo Primavera XML o Primavera XER que contiene varios proyectos utilizando las opciones de lectura de Primavera.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// Devuelve el proyecto con UID especial.
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Ver también

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

Inicializa una nueva instancia de la clase [`Project`](../) para leer datos de una base de datos especificada por la instancia de la clase [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/).

```csharp
public Project(DbSettings settings)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| settings | DbSettings | la instancia especificada de la clase [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/). |

## Ejemplos

Muestra cómo importar un proyecto desde una base de datos Primavera utilizando la configuración de la base de datos.

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

// Inicializa una nueva instancia de la clase PrimaveraDbSettings con la cadena de conexión y el ID del proyecto
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Inicializa una nueva instancia de la clase Project
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Ver también

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

Inicializa una nueva instancia de la clase [`Project`](../) a partir de una plantilla (archivo mpp o mpt existente).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | Flujo desde el cual cargar una plantilla. |
| parseErrorHandler | ParseErrorCallback | el método de devolución de llamada especificado para manejar errores de análisis XML. |

## Ejemplos

Muestra cómo leer un proyecto desde un archivo XML con caracteres inválidos.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // abra el flujo que contiene XML con intervalos de tiempo rotos
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

### Ver también

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

Inicializa una nueva instancia de la clase [`Project`](../) a partir de una plantilla (archivo mpp o mpt existente).

```csharp
public Project(Stream stream, string protectionPassword)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | Flujo desde el cual cargar una plantilla. |
| protectionPassword | Cadena | Contraseña de protección. |

## Observaciones

La lectura de archivos protegidos con contraseña actualmente solo es compatible con el formato de archivo MSP 2003.

## Ejemplos

Muestra cómo comprobar si el MPP está protegido con contraseña.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

Muestra cómo leer archivos MPP protegidos con contraseña desde un flujo.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

Inicializa una nueva instancia de la clase [`Project`](../) a partir de una plantilla (archivo mpp o mpt existente) con la instancia especificada de la clase [`LoadOptions`](../../loadoptions/).

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectTemplate | Cadena | Ruta a la plantilla desde la cual crear el proyecto |
| options | LoadOptions | la instancia especificada de la clase [`LoadOptions`](../../loadoptions/). |

## Ejemplos

Muestra cómo cargar el proyecto desde un archivo usando la instancia &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

Muestra cómo leer un proyecto desde un archivo XML de Primavera con error de análisis.

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

// Devuelve el proyecto con UID especial.
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

Inicializa una nueva instancia de la clase [`Project`](../) desde el flujo con la instancia especificada de la clase [`LoadOptions`](../../loadoptions/).

```csharp
public Project(Stream stream, LoadOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | Flujo del Project Streamclass |
| options | LoadOptions | la instancia especificada de la clase [`LoadOptions`](../../loadoptions/)clase |

## Ejemplos

Muestra cómo cargar el proyecto desde un flujo usando la instancia &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

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

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


