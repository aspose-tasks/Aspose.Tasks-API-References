---
title: "Project.OleObjects"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. OleObject 클래스의 인스턴스를 포함하는 컬렉션을 가져옵니다. 이 컬렉션은 이 프로젝트 파일에 연결되거나 포함된 것입니다. mpp 파일 형식에만 사용할 수 있습니다. 이 컬렉션은 Clear 작업을 제외하고는 읽기 전용입니다."
type: docs
weight: 700
url: /ko/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

[`OleObject`](../../oleobject/) 클래스의 인스턴스를 포함하는 컬렉션을 가져옵니다. 이 컬렉션은 프로젝트 파일에 연결되거나 포함된 것입니다. mpp 파일 형식에만 사용할 수 있습니다. 이 컬렉션은 'Clear' 작업을 제외하고는 읽기 전용입니다.

```csharp
public OleObjectCollection OleObjects { get; }
```

## 예제

임베드된 OLE 객체를 추출하는 방법을 보여줍니다.

```csharp
IDictionary<string, string> formatExt = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !formatExt.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + formatExt[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### 또 보기

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


