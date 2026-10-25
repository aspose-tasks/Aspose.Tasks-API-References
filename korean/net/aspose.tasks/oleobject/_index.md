---
title: "클래스 OleObject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OleObject 클래스. MPP 파일의 간트 차트 보기(Gantt Chart View)에 삽입될 수 있는 OLE 개체를 나타냅니다."
type: docs
weight: 1120
url: /ko/net/aspose.tasks/oleobject/
---
## OleObject class

MPP 파일의 Gantt Chart View에 삽입될 수 있는 OLE 객체를 나타냅니다.

```csharp
public class OleObject
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [OleObject](oleobject/)() | `OleObject` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | 삽입된 개체를 열 때 사용할 애플리케이션 이름을 가져오거나 설정합니다. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | 삽입된 파일의 데이터를 가져오거나 설정합니다; 데이터가 삽입되지 않은 경우 null입니다. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | OLE 개체를 아이콘으로 표시할지 일반 그림으로 표시할지 나타내는 플래그를 가져오거나 설정합니다. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | 삽입된 개체의 파일 형식을 가져오거나 설정합니다. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | 삽입된 개체의 전체 경로를 가져오거나 설정합니다. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | 개체 ID를 가져오거나 설정합니다. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | 삽입된 개체의 레이블을 가져오거나 설정합니다. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | 프로젝트 파일에 실제 데이터가 저장된 링크 소스에 대한 링크만 포함되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | OLE 개체 인스턴스의 이름을 가져오거나 설정합니다. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | 삽입된 개체의 임시 파일 경로를 가져오거나 설정합니다. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | 삽입된 개체가 속한 [`View`](./view/) 클래스의 인스턴스를 가져오거나 설정합니다. |

## 예제

OLE 개체에 대한 정보를 읽는 방법을 보여줍니다.

```csharp
[Test]
public void WorkWithOleObject()
{
    var images = new Project(DataDir + "TaskImage2010.mpp");
    List<OleObject> oleObjects = images.OleObjects.ToList();

    Console.WriteLine("Ole Objects Count: " + oleObjects.Count);
    foreach (var oleObject in oleObjects)
    {
        Console.WriteLine(" Id: " + oleObject.Id);
        Console.WriteLine(" Name: " + oleObject.Name);
        Console.WriteLine(" DisplayAsIcon: " + oleObject.DisplayAsIcon);
        Console.WriteLine(" Application Name: " + oleObject.ApplicationName);
        Console.WriteLine(" File Format: " + oleObject.FileFormat);
        Console.WriteLine(" Label: " + oleObject.Label);
        Console.WriteLine(" Full Path: " + oleObject.FullPath);
        Console.WriteLine(" Is Linked: " + oleObject.Linked);
        Console.WriteLine(" View Name: " + oleObject.View.Name);
        Console.WriteLine(" Content (first 10 bytes): " + this.Get10Bytes(oleObject));
    }
}

private string Get10Bytes(OleObject oleObject)
{
    byte[] bytes = oleObject.Content;
    var chunk = new byte[10];
    Array.Copy(bytes, chunk, 10);
    var builder = new StringBuilder();
    foreach (var b in chunk)
    {
        builder.Append(b + ", ");
    }

    builder.Remove(builder.Length - 3, 1);
    return builder.ToString();
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


