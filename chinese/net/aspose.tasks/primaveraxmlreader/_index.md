---
title: "类 PrimaveraXmlReader"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.PrimaveraXmlReader 类。表示一种读取器，可用于从 Primavera Xml 文件检索项目 UID。"
type: docs
weight: 1400
url: /zh/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

表示一个读取器，允许从 Primavera Xml 文件检索项目 UID。

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | 初始化 `PrimaveraXmlReader` 类的新实例。 |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | 初始化 `PrimaveraXmlReader` 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | 返回项目的简短信息对象列表。 |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | 返回项目唯一标识符的列表。 |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | 加载具有指定唯一标识符的项目。 |

## 示例

展示如何从 Primavera XML 文件检查短项目的信息。

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### 另见

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


