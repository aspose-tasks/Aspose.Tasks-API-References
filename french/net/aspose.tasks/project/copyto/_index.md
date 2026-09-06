---
title: "Project.CopyTo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode du projet. Copie les données principales et les propriétés du projet vers un autre projet"
type: docs
weight: 1060
url: /fr/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

Copie les données principales et les propriétés du projet vers un autre projet.

```csharp
public void CopyTo(Project another)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| un autre | Project | Un autre projet vers lequel copier les données. |

## Exemples

Montre comment copier les données du projet vers un autre projet.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// ignorer la copie des données de vue lors de la copie des données communes du projet.
project.CopyTo(mppProject);
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

Copie les données principales et les propriétés du projet vers un autre projet.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| un autre | Project | Un autre projet vers lequel copier les données. |
| options | CopyToOptions | Options de copie pour contrôler le processus de copie. |

## Exemples

Montre comment copier le projet en utilisant une instance &lt;see cref="Aspose.Tasks.CopyToOptions"/&gt;.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// ignorer la copie des données de vue lors de la copie des données communes du projet.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### Voir aussi

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


