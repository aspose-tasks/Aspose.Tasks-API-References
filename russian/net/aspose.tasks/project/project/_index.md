---
title: "Project.Project"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор Project. Инициализирует новый экземпляр класса Project."
type: docs
weight: 10
url: /ru/net/aspose.tasks/project/project/
---
## Project() {#constructor}

Инициализирует новый экземпляр класса [`Project`](../).

```csharp
public Project()
```

## Примеры

Показывает, как создать проект и сохранить его в формате MPP без использования шаблона MPP.

```csharp
var project = new Project();

// Проект будет сохранён в формате MPP с использованием внутреннего шаблона MPP.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

Инициализирует новый экземпляр класса [`Project`](../) из защищённого паролем шаблона (существующий файл mpp или mpt).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| projectTemplate | Строка | Путь к шаблону, из которого создаётся проект. |
| protectionPassword | Строка | Пароль защиты. |

## Примечания

Чтение файлов, защищённых паролем, в настоящее время поддерживается только для формата файлов MSP 2003.

## Примеры

Показывает, как читать файлы MPP, защищённые паролем.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

Инициализирует новый экземпляр класса [`Project`](../) из шаблона (существующий файл mpp или mpt).

```csharp
public Project(string projectTemplate)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| projectTemplate | Строка | Путь к шаблону, из которого создаётся проект. |

## Примеры

Показывает, как прочитать файл MPP.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

Инициализирует новый экземпляр класса [`Project`](../) из потока с указанным экземпляром класса [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток класса Project Streamclass |
| options | PrimaveraReadOptions | указанный экземпляр класса [`PrimaveraReadOptions`](../../primaverareadoptions/), который позволяет настраивать чтение форматов Primavera (XER или XML). |

## Примеры

Показывает, как прочитать проект из потока с файлом Primavera XML или Primavera XER, содержащим несколько проектов.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // Возвращает проект со специальным UID
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### См. также

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

Инициализирует новый экземпляр класса [`Project`](../) из шаблона (существующий файл mpp или mpt).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| projectTemplate | Строка | Путь к шаблону, из которого создаётся проект. |
| parseErrorHandler | ParseErrorCallback | указанный метод обратного вызова для обработки ошибок разбора xml. |

## Примеры

Показывает, как прочитать проект из потока с XML‑файлом, содержащим недопустимые символы.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // откройте файл, содержащий XML с повреждёнными временными интервалами
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

### См. также

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

Инициализирует новый экземпляр класса [`Project`](../) из потока.

```csharp
public Project(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток, из которого загружается шаблон. |

## Примеры

Показывает, как прочитать XML‑файл проекта из потока.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

Инициализирует новый экземпляр класса [`Project`](../) из экземпляра StreamReader.

```csharp
public Project(StreamReader reader)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| reader | StreamReader | Потоковый читатель, из которого загружается шаблон. |

## Примеры

Показывает, как читать файлы MPX с определённой кодировкой.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

Инициализирует новый экземпляр класса [`Project`](../) из шаблона (существующего файла MPP или MPT) с указанным экземпляром класса [`PrimaveraReadOptions`](../../primaverareadoptions/).

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| projectTemplate | Строка | Путь к шаблону, из которого создаётся проект |
| options | PrimaveraReadOptions | указанный экземпляр класса [`PrimaveraReadOptions`](../../primaverareadoptions/). |

## Примеры

Показывает, как прочитать проект из файла Primavera XML или Primavera XER, содержащего несколько проектов, используя параметры чтения Primavera.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// Возвращает проект со специальным UID
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### См. также

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

Инициализирует новый экземпляр класса [`Project`](../) для чтения данных из базы данных, указанной экземпляром класса [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/).

```csharp
public Project(DbSettings settings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| settings | DbSettings | указанный экземпляр класса [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/). |

## Примеры

Показывает, как импортировать проект из базы данных Primavera, используя настройки базы данных.

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

// Инициализировать новый экземпляр класса PrimaveraDbSettings с строкой подключения и идентификатором проекта
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Инициализировать новый экземпляр класса Project
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### См. также

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

Инициализирует новый экземпляр класса [`Project`](../) из шаблона (существующего файла mpp или mpt).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток, из которого загружается шаблон. |
| parseErrorHandler | ParseErrorCallback | указанный метод обратного вызова для обработки ошибок разбора xml. |

## Примеры

Показывает, как прочитать проект из XML‑файла с недопустимыми символами.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // откройте поток, содержащий XML с повреждёнными диапазонами времени
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

### См. также

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

Инициализирует новый экземпляр класса [`Project`](../) из шаблона (существующего файла mpp или mpt).

```csharp
public Project(Stream stream, string protectionPassword)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток, из которого загружается шаблон. |
| protectionPassword | Строка | Пароль защиты. |

## Примечания

Чтение файлов, защищённых паролем, в настоящее время поддерживается только для формата файлов MSP 2003.

## Примеры

Показывает, как проверить, защищён ли MPP паролем.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

Показывает, как прочитать защищённые паролем файлы MPP из потока.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

Инициализирует новый экземпляр класса [`Project`](../) из шаблона (существующего файла mpp или mpt) с указанным экземпляром класса [`LoadOptions`](../../loadoptions/).

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| projectTemplate | Строка | Путь к шаблону, из которого создаётся проект |
| options | LoadOptions | указанный экземпляр класса [`LoadOptions`](../../loadoptions/). |

## Примеры

Показывает, как загрузить проект из файла, используя экземпляр &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

Показывает, как прочитать проект из XML‑файла Primavera с ошибкой разбора.

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

// Возвращает проект со специальным UID
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### См. также

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

Инициализирует новый экземпляр класса [`Project`](../) из потока с указанным экземпляром класса [`LoadOptions`](../../loadoptions/).

```csharp
public Project(Stream stream, LoadOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток класса Project Streamclass |
| options | LoadOptions | указанный экземпляр класса [`LoadOptions`](../../loadoptions/). |

## Примеры

Показывает, как загрузить проект из потока, используя экземпляр &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

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

### См. также

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


