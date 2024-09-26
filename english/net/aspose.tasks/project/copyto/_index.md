---
title: Project.CopyTo
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Copies projects main data and properties to another project
type: docs
weight: 1050
url: /net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

Copies project's main data and properties to another project.

```csharp
public void CopyTo(Project another)
```

| Parameter | Type | Description |
| --- | --- | --- |
| another | Project | Another project to copy data to. |

## Examples

Shows how to copy the project data to another project.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// skip copying of view data while copying common project data.
project.CopyTo(mppProject);
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

Copies project's main data and properties to another project.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| another | Project | Another project to copy data to. |
| options | CopyToOptions | Copy options to control copy process. |

## Examples

Shows how to copy the project with usage of &lt;see cref="Aspose.Tasks.CopyToOptions"/&gt; instance.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// skip copying of view data while copying common project data.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### See Also

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


