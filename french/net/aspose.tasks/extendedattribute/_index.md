---
title: Class ExtendedAttribute
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.ExtendedAttribute classe. Représente les attributs étendus.
type: docs
weight: 520
url: /fr/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Représente les attributs étendus.

```csharp
public class ExtendedAttribute
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Obtient la définition d'attribut. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Obtient ou définit une valeur pour les attributs avec des types de date (Date, Début, Fin). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | Obtient ou définit la valeur des attributs de type "Durée". |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Obtient l'identifiant d'un champ. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | Obtient ou définit une valeur indiquant si un indicateur est défini pour un attribut de type 'Flag'. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Obtient si le calcul de la valeur de l'attribut étendu a entraîné une erreur. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Obtient ou définit une valeur pour les attributs avec des types numériques (coût, nombre). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | Obtient ou définit une valeur pour les attributs de type "Texte". |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Obtient le guid d'une valeur de recherche. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Obtient une valeur indiquant si une valeur de ce`ExtendedAttribute` l'instance est en lecture seule.  renvoie true si une formule ou un cumul est défini dans le[`ExtendedAttributeDefinition`](../extendedattributedefinition/) pour cet objet. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Renvoie la représentation sous forme de chaîne courte d'un attribut étendu. |

### Remarques

Actuellement pris en charge tous les types d'attributs étendus lus à partir de MSP Xml 2003/2007 et mpp 2003. Pour MSP mpp 2007, tous les attributs étendus lus sont pris en charge, à l'exception des durées et des drapeaux.

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks/)
* Assemblée [Aspose.Tasks](../../)


