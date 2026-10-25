---
title: "Project.Project"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 构造函数。初始化 Project 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/project/project/
---
## Project() {#constructor}

初始化一个 [`Project`](../) 类的新实例。

```csharp
public Project()
```

## 示例

展示如何创建项目并保存为 MPP 格式，而无需提供 MPP 模板文件。

```csharp
var project = new Project();

// 项目将使用内部 MPP 模板保存为 MPP。
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

从受密码保护的模板（现有的 mpp 或 mpt 文件）初始化一个 [`Project`](../) 类的新实例。

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | 字符串 | 用于创建项目的模板路径。 |
| protectionPassword | 字符串 | 保护密码。 |

## 备注

当前仅支持读取受密码保护的 MSP 2003 文件格式。

## 示例

展示如何读取受密码保护的 MPP 文件。

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

从模板（现有的 mpp 或 mpt 文件）初始化一个 [`Project`](../) 类的新实例。

```csharp
public Project(string projectTemplate)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | 字符串 | 用于创建项目的模板路径。 |

## 示例

展示如何读取 MPP 文件。

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

使用指定的 [`PrimaveraReadOptions`](../../primaverareadoptions/) 类实例，从流中初始化一个 [`Project`](../) 类的新实例。

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | Project Streamclass 的流 |
| options | PrimaveraReadOptions | 指定的 [`PrimaveraReadOptions`](../../primaverareadoptions/) 类实例，允许自定义 Primavera 格式（XER 或 XML）的读取。 |

## 示例

展示如何从流中读取项目，使用包含多个项目的 Primavera XML 或 Primavera XER 文件。

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // 返回具有特殊 UID 的项目
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### 另见

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

从模板（现有的 mpp 或 mpt 文件）初始化一个 [`Project`](../) 类的新实例。

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | 字符串 | 用于创建项目的模板路径。 |
| parseErrorHandler | ParseErrorCallback | 指定的回调方法，用于处理 xml 解析错误。 |

## 示例

展示如何从包含无效字符的 XML 文件的流中读取项目。

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // 打开包含损坏时间跨度的 XML 文件。
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

### 另见

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

从流中初始化 [`Project`](../) 类的新实例。

```csharp
public Project(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 用于加载模板的流。 |

## 示例

展示如何从流中读取 XML 项目文件。

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

从 StreamReader 实例初始化 [`Project`](../) 类的新实例。

```csharp
public Project(StreamReader reader)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| reader | StreamReader | 用于加载模板的流读取器。 |

## 示例

展示如何使用特定编码读取 MPX 文件。

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

使用指定的 [`PrimaveraReadOptions`](../../primaverareadoptions/) 类实例，从模板（现有的 MPP 或 MPT 文件）初始化 [`Project`](../) 类的新实例。

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | 字符串 | 用于创建项目的模板路径 |
| options | PrimaveraReadOptions | 指定的 [`PrimaveraReadOptions`](../../primaverareadoptions/) 类实例。 |

## 示例

展示如何使用 Primavera 读取选项，从包含多个项目的 Primavera XML 或 Primavera XER 文件读取项目。

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// 返回具有特殊 UID 的项目
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### 另见

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

初始化 [`Project`](../) 类的新实例，以从由 [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) 类实例指定的数据库读取数据。

```csharp
public Project(DbSettings settings)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| settings | DbSettings | 指定的 [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) 类实例。 |

## 示例

展示如何使用数据库设置从 Primavera 数据库导入项目。

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

// 使用连接字符串和项目 id 初始化 PrimaveraDbSettings 类的新实例
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// 初始化 Project 类的新实例
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### 另见

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

从模板（现有的 mpp 或 mpt 文件）初始化 [`Project`](../) 类的新实例。

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 用于加载模板的流。 |
| parseErrorHandler | ParseErrorCallback | 指定的回调方法，用于处理 xml 解析错误。 |

## 示例

展示如何从包含无效字符的 XML 文件中读取项目。

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // 打开包含时间跨度损坏的 XML 的流
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

### 另见

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

从模板（现有的 mpp 或 mpt 文件）初始化 [`Project`](../) 类的新实例。

```csharp
public Project(Stream stream, string protectionPassword)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 用于加载模板的流。 |
| protectionPassword | 字符串 | 保护密码。 |

## 备注

当前仅支持读取受密码保护的 MSP 2003 文件格式。

## 示例

展示如何检查 MPP 是否受密码保护。

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

展示如何从流中读取受密码保护的 MPP 文件。

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

使用指定的 [`LoadOptions`](../../loadoptions/) 类实例，从模板（现有的 mpp 或 mpt 文件）初始化一个新的 [`Project`](../) 类实例。

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | 字符串 | 用于创建项目的模板路径 |
| options | LoadOptions | 指定的 [`LoadOptions`](../../loadoptions/) 类实例。 |

## 示例

展示如何通过使用 &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt; 实例从文件加载项目。

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

展示如何从 Primavera XML 文件中读取项目（解析错误）。

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

// 返回具有特殊 UID 的项目
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### 另见

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

使用指定的 [`LoadOptions`](../../loadoptions/) 类实例，从流中初始化一个新的 [`Project`](../) 类实例。

```csharp
public Project(Stream stream, LoadOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | Project Streamclass 的流 |
| options | LoadOptions | 指定的 [`LoadOptions`](../../loadoptions/)class 实例 |

## 示例

展示如何通过使用 &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt; 实例从流加载项目。

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

### 另见

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


