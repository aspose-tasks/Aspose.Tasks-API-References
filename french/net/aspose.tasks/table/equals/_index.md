---
title: "Table.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Table. Retourne une valeur indiquant si cette instance est égale à un objet spécifié"
type: docs
weight: 120
url: /fr/net/aspose.tasks/table/equals/
---
## Table.Equals method

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | L'objet à comparer avec cette instance. |

### Valeur de retour

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## Exemples

Montre comment vérifier l'égalité des tables.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// L'égalité des tables est vérifiée par rapport à l'UID de la table.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### Voir aussi

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


