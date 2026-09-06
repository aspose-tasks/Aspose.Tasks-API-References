---
title: "OutlineCodeDefinition.FieldName"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "OutlineCodeDefinition propriété. Obtient ou définit le nom d'un code de contour personnalisé"
type: docs
weight: 70
url: /fr/net/aspose.tasks/outlinecodedefinition/fieldname/
---
## OutlineCodeDefinition.FieldName property

Obtient ou définit le nom d'un code de plan personnalisé.

```csharp
public string FieldName { get; set; }
```

## Exemples

Montre comment travailler avec les définitions de code de contour.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// créer une nouvelle définition de code de contour
var outline = new OutlineCodeDefinition();

// définir le numéro de champ d'un code de contour
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// définir le nom d'un code de contour personnalisé
outline.FieldName = "Outline Code1";

// définir le GUID d'un code de contour
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// définir une valeur indiquant si les valeurs spécifiées dans ce champ de code de contour doivent être des valeurs feuille
outline.LeafOnly = false;

// définir l'alias d'un code de contour personnalisé
outline.Alias = "My Outline Code";

// définir la prononciation phonétique de l'alias du code de contour personnalisé
outline.PhoneticAlias = "Outline Code";

// définir une valeur indiquant si les nouveaux codes doivent avoir tous les niveaux. Non disponible pour les codes d'entreprise.
outline.AllLevelsRequired = true;

// définir une valeur indiquant si un code de contour personnalisé est un code de contour personnalisé d'entreprise
outline.Enterprise = false;

// définir une référence à un autre champ personnalisé pour lequel cette définition de code de contour est un alias
outline.EnterpriseOutlineCodeAlias = 0;

// ajouter un masque de contour
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// définir une valeur indiquant si les valeurs spécifiées doivent provenir de la table des valeurs
outline.OnlyTableValuesAllowed = false;

// définir une valeur indiquant si le code de contour personnalisé peut être utilisé
// par l'assistant de substitution de ressources dans Microsoft Project
outline.ResourceSubstitutionEnabled = false;

// définir une valeur indiquant si les retraits de ce code de contour doivent être affichés.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Voir aussi

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


