---
title: "Asn.Resume"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La fecha en que se reanuda la asignación"
type: docs
weight: 490
url: /es/net/aspose.tasks/asn/resume/
---
## Asn.Resume field

La fecha en que se reanuda la asignación.

```csharp
public static readonly Key<DateTime, AsnKey> Resume;
```

## Ejemplos

Muestra cómo leer las fechas de detención/reanudación de la asignación.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// Imprime las fechas de detención y reanudación de la asignación de recursos
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


