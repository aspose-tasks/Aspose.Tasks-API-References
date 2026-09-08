---
title: "OleObjectCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OleObjectCollection 메서드. 이 컬렉션에 대한 열거자를 반환합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/oleobjectcollection/getenumerator/
---
## OleObjectCollection.GetEnumerator method

이 컬렉션에 대한 열거자를 반환합니다.

```csharp
public IEnumerator<OleObject> GetEnumerator()
```

### 반환 값

이 컬렉션에 대한 열거자.

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

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


