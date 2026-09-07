---
title: "VbaModuleAttribute.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo VbaModuleAttribute. Restituisce un valore che indica se questa istanza è uguale all'oggetto VbaModuleAttribute specificato"
type: docs
weight: 30
url: /it/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

Restituisce un valore che indica se questa istanza è uguale all'oggetto [`VbaModuleAttribute`](../) specificato.

```csharp
public bool Equals(VbaModuleAttribute other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | VbaModuleAttribute | L'oggetto [`VbaModuleAttribute`](../) specificato da confrontare con questa istanza. |

### Valore di ritorno

Restituisce true se questa istanza è uguale all'oggetto [`VbaModuleAttribute`](../) specificato; altrimenti, false.

## Esempi

Mostra come verificare l'uguaglianza degli attributi del modulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Vedi anche

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Restituisce un valore che indica se questa istanza è uguale all'oggetto [`VbaModuleAttribute`](../) specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | L'oggetto [`VbaModuleAttribute`](../) specificato da confrontare con questa istanza. |

### Valore di ritorno

Restituisce true se questa istanza è uguale all'oggetto [`VbaModuleAttribute`](../) specificato; altrimenti, false.

## Esempi

Mostra come verificare l'uguaglianza degli attributi del modulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Vedi anche

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


