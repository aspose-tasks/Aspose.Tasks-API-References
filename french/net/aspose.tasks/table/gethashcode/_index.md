---
title: "Table.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Table. Retourne un code de hachage pour cette Table"
type: docs
weight: 130
url: /fr/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

Renvoie un code de hachage pour cette Table.

```csharp
public override int GetHashCode()
```

### Valeur de retour

Renvoie une valeur de code de hachage pour cet objet.

## Exemples

Montre comment obtenir un code de hachage d'une table.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// Le code de hachage d'une table est égal à l'UID de la table
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### Voir aussi

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


