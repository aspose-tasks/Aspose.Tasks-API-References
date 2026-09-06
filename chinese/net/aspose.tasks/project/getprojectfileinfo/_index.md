---
title: "Project.GetProjectFileInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。读取项目文件信息"
type: docs
weight: 1280
url: /zh/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

从文件读取项目文件信息。

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件名 | 字符串 | 项目文件名。 |

### 返回值

项目文件信息 [`ProjectFileInfo`](../../projectfileinfo/)。

## 示例

展示如何从 XML 文件读取项目文件信息。

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 另见

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

从流中获取项目文件信息。

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 数据流。 |

### 返回值

项目文件信息 [`ProjectFileInfo`](../../projectfileinfo/)。

## 示例

展示如何从流中读取 XML 文件的项目文件信息。

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### 另见

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


