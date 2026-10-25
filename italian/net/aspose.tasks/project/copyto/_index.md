---
title: "Project.CopyTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo di Project. Copia i dati principali e le proprietà del progetto in un altro progetto"
type: docs
weight: 1060
url: /it/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

Copia i dati principali e le proprietà del progetto in un altro progetto.

```csharp
public void CopyTo(Project another)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| un altro | Project | Un altro progetto a cui copiare i dati. |

## Esempi

Mostra come copiare i dati del progetto in un altro progetto.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// ignora la copia dei dati della vista durante la copia dei dati comuni del progetto.
project.CopyTo(mppProject);
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

Copia i dati principali e le proprietà del progetto in un altro progetto.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| un altro | Project | Un altro progetto a cui copiare i dati. |
| opzioni | CopyToOptions | Opzioni di copia per controllare il processo di copia. |

## Esempi

Mostra come copiare il progetto utilizzando l'istanza &lt;see cref=\"Aspose.Tasks.CopyToOptions\"/&gt;.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// ignora la copia dei dati della vista durante la copia dei dati comuni del progetto.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### Vedi anche

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


