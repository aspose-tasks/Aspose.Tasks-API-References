---
title: "Asn.HyperlinkAddress"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La dirección de un hipervínculo asociado a la asignación"
type: docs
weight: 290
url: /es/net/aspose.tasks/asn/hyperlinkaddress/
---
## Asn.HyperlinkAddress field

La dirección de un hipervínculo asociado a la asignación.

```csharp
public static readonly Key<string, AsnKey> HyperlinkAddress;
```

## Observaciones

La dirección completa (Hipervínculo Href en Microsoft Project) del hipervínculo es una concatenación de HyperlinkAddress y HyperlinkSubAddress.

## Ejemplos

Muestra cómo leer/escribir las propiedades del hipervínculo.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Hyperlink, "Click to visit our site");
assignment.Set(Asn.HyperlinkAddress, "https://products.aspose.com");
assignment.Set(Asn.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + assignment.Get(Asn.Hyperlink));
Console.WriteLine("Hyperlink Address: " + assignment.Get(Asn.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + assignment.Get(Asn.HyperlinkSubAddress));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


