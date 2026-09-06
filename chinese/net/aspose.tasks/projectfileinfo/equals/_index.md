---
title: "ProjectFileInfo.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectFileInfo 方法。返回一个值，指示此实例是否等于指定的对象"
type: docs
weight: 50
url: /zh/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

返回一个值，指示此实例是否等于指定的对象。

```csharp
public bool Equals(ProjectFileInfo other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 其他 | ProjectFileInfo | 指定的对象，用于与此实例比较。 |

### 返回值

如果指定的 ProjectFileInfo 与此实例具有相同的文件格式和应用信息，则返回 true。

## 示例

展示如何读取项目文件信息。

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 另见

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

返回一个值，指示此实例是否等于指定的对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 指定的对象，用于与此实例比较。 |

### 返回值

如果指定的 ProjectFileInfo 与此实例具有相同的文件格式和应用信息，则返回 true。

## 示例

展示如何读取项目文件信息。

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 另见

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


