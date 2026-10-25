---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo PrimaveraBaseReader. Carica il progetto con l'identificatore univoco specificato"
type: docs
weight: 30
url: /it/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Carica il progetto con l'identificatore univoco specificato.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectUid | Int32 | Identificatore univoco del progetto da caricare. |

### Valore di ritorno

Progetto con l'identificatore univoco specificato dal file multi-progetto specificato. Null se il progetto non esiste.

## Esempi

Mostra come caricare un progetto da un file XML Primavera quando l'uid del progetto è noto.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

Mostra come esaminare le informazioni dei progetti brevi da un file Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### Vedi anche

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


