---
title: "类 OleObject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OleObject 类。表示可以插入到 MPP 文件的甘特图视图中的 OLE 对象。"
type: docs
weight: 1120
url: /zh/net/aspose.tasks/oleobject/
---
## OleObject class

表示可以插入到 MPP 文件的 Gantt Chart 视图中的 OLE 对象。

```csharp
public class OleObject
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [OleObject](oleobject/)() | 初始化 `OleObject` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | 获取或设置用于打开嵌入对象的应用程序名称。 |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | 获取或设置嵌入文件的数据；如果未嵌入数据则为 null。 |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | 获取或设置一个标志，指示 OLE 对象应显示为图标还是其常规图片。 |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | 获取或设置嵌入对象的文件格式。 |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | 获取或设置已插入对象的完整路径。 |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | 获取或设置对象 ID。 |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | 获取或设置已插入对象的标签。 |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | 获取一个值，指示项目文件是否仅包含指向链接源中实际数据的链接。 |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | 获取或设置 OLE 对象实例的名称。 |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | 获取或设置已插入对象的临时文件路径。 |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | 获取或设置已插入对象所属的 [`View`](./view/) 类实例。 |

## 示例

展示如何读取 OLE 对象的信息。

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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


