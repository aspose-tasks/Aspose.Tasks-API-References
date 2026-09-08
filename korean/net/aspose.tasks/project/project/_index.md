---
title: "Project.Project"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 생성자. Project 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/project/project/
---
## Project() {#constructor}

[`Project`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Project()
```

## 예제

MPP 템플릿 파일을 전달하지 않고 프로젝트를 생성하고 MPP 형식으로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 프로젝트는 내부 MPP 템플릿을 사용하여 MPP 형식으로 저장됩니다.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

비밀번호로 보호된 템플릿(존재하는 mpp 또는 mpt 파일)에서 [`Project`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | 문자열 | 프로젝트를 생성할 템플릿 경로. |
| protectionPassword | 문자열 | 보호 비밀번호. |

## 비고

현재 비밀번호로 보호된 파일 읽기는 MSP 2003 파일 형식에만 지원됩니다.

## 예제

비밀번호로 보호된 MPP 파일을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

템플릿(존재하는 mpp 또는 mpt 파일)에서 [`Project`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Project(string projectTemplate)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | 문자열 | 프로젝트를 생성할 템플릿 경로. |

## 예제

MPP 파일을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

지정된 [`PrimaveraReadOptions`](../../primaverareadoptions/) 클래스 인스턴스를 사용하여 스트림에서 [`Project`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 프로젝트 Streamclass의 스트림 |
| options | PrimaveraReadOptions | Primavera 형식(XER 또는 XML) 읽기를 사용자 정의할 수 있게 하는 지정된 [`PrimaveraReadOptions`](../../primaverareadoptions/) 클래스 인스턴스. |

## 예제

여러 프로젝트를 포함하는 Primavera XML 또는 Primavera XER 파일을 사용하여 스트림에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // 특수 UID를 가진 프로젝트를 반환합니다.
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### 또 보기

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

템플릿(존재하는 mpp 또는 mpt 파일)에서 [`Project`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | 문자열 | 프로젝트를 생성할 템플릿 경로. |
| parseErrorHandler | ParseErrorCallback | xml 구문 오류를 처리하기 위한 지정된 콜백 메서드. |

## 예제

잘못된 문자를 포함한 XML 파일이 있는 스트림에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // 손상된 기간이 있는 XML을 포함하는 파일을 엽니다.
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

### 또 보기

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

스트림에서 [`Project`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Project(Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 템플릿을 로드할 스트림. |

## 예제

스트림에서 XML 프로젝트 파일을 읽는 방법을 보여줍니다.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

`StreamReader` 인스턴스에서 [`Project`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Project(StreamReader reader)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| reader | StreamReader | 템플릿을 로드할 스트림 리더. |

## 예제

특정 인코딩으로 MPX 파일을 읽는 방법을 보여줍니다.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

템플릿(기존 MPP 또는 MPT 파일)과 지정된 [`PrimaveraReadOptions`](../../primaverareadoptions/) 클래스 인스턴스를 사용하여 [`Project`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | 문자열 | 프로젝트를 생성할 템플릿 경로 |
| options | PrimaveraReadOptions | 지정된 [`PrimaveraReadOptions`](../../primaverareadoptions/) 클래스 인스턴스. |

## 예제

Primavera 읽기 옵션을 사용하여 여러 프로젝트를 포함하는 Primavera XML 또는 Primavera XER 파일에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// 특수 UID를 가진 프로젝트를 반환합니다.
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### 또 보기

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

지정된 [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) 클래스 인스턴스로 지정된 데이터베이스에서 데이터를 읽기 위해 [`Project`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Project(DbSettings settings)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| settings | DbSettings | 지정된 [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) 클래스 인스턴스. |

## 예제

데이터베이스 설정을 사용하여 Primavera 데이터베이스에서 프로젝트를 가져오는 방법을 보여줍니다.

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

// 연결 문자열과 프로젝트 ID를 사용하여 PrimaveraDbSettings 클래스의 새 인스턴스를 초기화합니다.
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Project 클래스의 새 인스턴스를 초기화합니다.
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### 또 보기

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

[`Project`](../) 클래스의 새 인스턴스를 템플릿(기존 mpp 또는 mpt 파일)에서 초기화합니다.

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 템플릿을 로드할 스트림. |
| parseErrorHandler | ParseErrorCallback | xml 구문 오류를 처리하기 위한 지정된 콜백 메서드. |

## 예제

잘못된 문자가 포함된 XML 파일에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // 손상된 기간이 있는 XML을 포함하는 스트림을 엽니다.
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

### 또 보기

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

[`Project`](../) 클래스의 새 인스턴스를 템플릿(기존 mpp 또는 mpt 파일)에서 초기화합니다.

```csharp
public Project(Stream stream, string protectionPassword)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 템플릿을 로드할 스트림. |
| protectionPassword | 문자열 | 보호 비밀번호. |

## 비고

현재 비밀번호로 보호된 파일 읽기는 MSP 2003 파일 형식에만 지원됩니다.

## 예제

MPP가 비밀번호로 보호되는지 확인하는 방법을 보여줍니다.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

스트림에서 비밀번호로 보호된 MPP 파일을 읽는 방법을 보여줍니다.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

[`Project`](../) 클래스의 새 인스턴스를 템플릿(존재하는 mpp 또는 mpt 파일)에서 지정된 [`LoadOptions`](../../loadoptions/) 클래스 인스턴스를 사용하여 초기화합니다.

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectTemplate | 문자열 | 프로젝트를 생성할 템플릿 경로 |
| options | LoadOptions | 지정된 [`LoadOptions`](../../loadoptions/) 클래스. |

## 예제

파일에서 프로젝트를 로드하는 방법을 &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt; 인스턴스를 사용하여 보여줍니다.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

오류가 발생한 파싱을 포함한 Primavera XML 파일에서 프로젝트를 읽는 방법을 보여줍니다.

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

// 특수 UID를 가진 프로젝트를 반환합니다.
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

### 또 보기

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

[`Project`](../) 클래스의 새 인스턴스를 스트림에서 지정된 [`LoadOptions`](../../loadoptions/) 클래스 인스턴스를 사용하여 초기화합니다.

```csharp
public Project(Stream stream, LoadOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 프로젝트 Streamclass의 스트림 |
| options | LoadOptions | 지정된 [`LoadOptions`](../../loadoptions/)class 인스턴스 |

## 예제

스트림에서 프로젝트를 로드하는 방법을 &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt; 인스턴스를 사용하여 보여줍니다.

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

### 또 보기

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


