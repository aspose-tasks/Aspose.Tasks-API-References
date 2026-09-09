---
title: "Project.CopyTo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Projenin ana veri ve özelliklerini başka bir projeye kopyalar"
type: docs
weight: 1060
url: /tr/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar.

```csharp
public void CopyTo(Project another)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başka | Project | Veri kopyalanacak başka bir proje. |

## Örnekler

Proje verilerini başka bir projeye nasıl kopyalayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// Ortak proje verileri kopyalanırken görünüm verilerinin kopyalanmasını atla.
project.CopyTo(mppProject);
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

Projenin ana verilerini ve özelliklerini başka bir projeye kopyalar.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başka | Project | Veri kopyalanacak başka bir proje. |
| seçenekler | CopyToOptions | Kopyalama sürecini kontrol etmek için kopyalama seçenekleri. |

## Örnekler

Projeyi &lt;see cref="Aspose.Tasks.CopyToOptions"/&gt; örneği kullanarak nasıl kopyalayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// Ortak proje verileri kopyalanırken görünüm verilerinin kopyalanmasını atla.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### Ayrıca Bakınız

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


