---
title: "Project.Save"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 지정된 저장 옵션을 사용하여 문서를 파일에 저장합니다."
type: docs
weight: 1200
url: /ko/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

지정된 저장 옵션을 사용하여 문서를 파일에 저장합니다.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 파일명 | 문자열 | 파일 이름. |
| 옵션 | SimpleSaveOptions | 저장 옵션. |

## 예제

프로젝트를 MPP 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### 또 보기

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

프로젝트 데이터를 파일에 저장합니다.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 파일명 | 문자열 | 파일 이름. |
| 형식 | SaveFileFormat | 저장 파일 형식. |

## 예제

MPP 템플릿 파일을 전달하지 않고 프로젝트를 생성하고 MPP 형식으로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 프로젝트는 내부 MPP 템플릿을 사용하여 MPP 형식으로 저장됩니다.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

프로젝트 데이터를 mpp 형식 파일에 저장합니다.

```csharp
public void Save(string filename)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 파일명 | 문자열 | 파일 이름. |

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

지정된 저장 옵션을 사용하여 프로젝트를 스트림에 저장합니다.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 스트림. |
| 옵션 | SimpleSaveOptions | 저장 옵션. |

## 예제

MPP 저장 옵션을 사용하여 프로젝트를 스트림에 MPP 파일로 저장하는 방법을 보여줍니다.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // MPPSaveOptions를 사용하여 MPP 형식으로 저장합니다.
    project.Save(stream, options);
}
```

프로젝트를 스트림에 이미지로 저장하고 이미지 옵션을 제어하는 방법을 보여줍니다.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // ImageSaveOptions를 사용하여 프로젝트를 이미지 형식으로 저장합니다.
    project.Save(stream, options);
}
```

### 또 보기

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

프로젝트 데이터를 스트림에 저장합니다.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 스트림. |
| format | SaveFileFormat | 지정된 저장 파일 형식.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## 예제

프로젝트를 스트림에 XML MS Project 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // 스트림을 XML 형식으로 씁니다.
    project.Save(stream, SaveFileFormat.Xml);
}
```

### 또 보기

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


