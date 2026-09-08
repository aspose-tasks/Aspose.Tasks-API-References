---
title: "클래스 OleObjectCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OleObjectCollection 클래스. OleObject 클래스의 인스턴스를 포함하는 컬렉션을 나타냅니다."
type: docs
weight: 1130
url: /ko/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

[`OleObject`](../oleobject/) 클래스의 인스턴스를 포함하는 컬렉션을 나타냅니다.

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | 컬렉션을 비웁니다. 이러한 변경 사항을 지속하려면 new MPPSaveOptions { WriteViewData = true; }와 함께 project.Save를 호출해야 합니다. |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | `OleObjectCollection` 클래스의 인스턴스를 [`OleObject`](../oleobject/) 클래스의 인스턴스를 포함하는 리스트로 변환합니다. |

## 예제

OLE 객체 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// 인덱스 접근을 사용하여
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// 또는 열거를 통해 OLE 객체를 반복할 수 있습니다
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### 또 보기

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


