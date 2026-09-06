---
title: "Project.CopyTo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。将项目的主要数据和属性复制到另一个项目"
type: docs
weight: 1060
url: /zh/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

将项目的主要数据和属性复制到另一个项目。

```csharp
public void CopyTo(Project another)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 另一个 | Project | 要复制数据到的另一个项目。 |

## 示例

展示如何将项目数据复制到另一个项目。

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// 在复制通用项目数据时跳过视图数据的复制。
project.CopyTo(mppProject);
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

将项目的主要数据和属性复制到另一个项目。

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 另一个 | Project | 要复制数据到的另一个项目。 |
| 选项 | CopyToOptions | 复制选项以控制复制过程。 |

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.CopyToOptions\"/&gt; 实例来复制项目。

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// 在复制通用项目数据时跳过视图数据的复制。
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### 另见

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


