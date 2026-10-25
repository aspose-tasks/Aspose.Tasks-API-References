---
title: "OleObject.DisplayAsIcon"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OleObject 속성. OLE 객체를 아이콘으로 표시할지 일반 이미지로 표시할지 나타내는 플래그를 가져오거나 설정합니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

OLE 개체를 아이콘으로 표시할지 일반 그림으로 표시할지 나타내는 플래그를 가져오거나 설정합니다.

```csharp
public bool DisplayAsIcon { get; set; }
```

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

* class [OleObject](../)
* namespace [Aspose.Tasks](../../oleobject/)
* assembly [Aspose.Tasks](../../../)


