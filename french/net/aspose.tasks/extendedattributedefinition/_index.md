---
title: ExtendedAttributeDefinition
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Représente une définition dattribut étendue associée à un projet.
type: docs
weight: 530
url: /fr/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Représente une définition d'attribut étendue associée à un projet.

```csharp
public class ExtendedAttributeDefinition
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias) { get; set; } | Obtient ou définit l'alias d'un champ personnalisé. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues) { get; set; } | Obtient ou définit une valeur indiquant si les nouvelles valeurs ajoutées à un projet sont automatiquement ajoutées à la liste. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown) { get; set; } | Obtient ou définit une valeur indiquant si un déploiement automatique des devoirs est activé. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype) { get; set; } | Obtient ou définit le type de calcul de la valeur de l'attribut personnalisé. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype) { get; } | Obtient le type d'un champ personnalisé. |
| [Default](../../aspose.tasks/extendedattributedefinition/default) { get; set; } | Obtient ou définit la valeur par défaut dans la liste. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid) { get; set; } | Obtient ou définit le Guid de l'entrée de table de recherche par défaut. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype) { get; set; } | Obtient ou définit l'attribut étendu est associé à une tâche, une ressource ou une affectation. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid) { get; set; } | Obtient ou définit correspond à l'ID de projet d'un champ personnalisé. Utilise la représentation sous forme de chaîne d'une constante à partir de[`ExtendedAttributeTask`](../extendedattributetask) classe à préciser[`FieldId`](./fieldid) propriété. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname) { get; } | Obtient le nom d'un champ personnalisé. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula) { get; set; } | Obtient ou définit la formule que Microsoft Project utilise pour remplir un champ de tâche personnalisé. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid) { get; set; } | Obtient ou définit le Guid d'un champ personnalisé. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid) { get; } | Obtient un Guid de la table de recherche associée à un champ personnalisé. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues) { get; set; } | Obtient ou définit le nombre maximal de valeurs que vous pouvez définir dans une liste de sélection. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject) { get; } | Obtient le projet parent pour le[`ExtendedAttributeDefinition`](../extendedattributedefinition) instance. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias) { get; set; } | Obtient ou définit la prononciation phonétique de l'alias d'un champ personnalisé. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues) { get; set; } | Obtient ou définit une valeur indiquant si les valeurs du champ personnalisé sont limitées aux valeurs du[`ValueList`](./valuelist) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype) { get; set; } | Obtient ou définit la manière dont les cumuls sont calculés. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid) { get; set; } | Obtient ou définit le GUID secondaire de l'attribut étendu. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid) { get; set; } | Obtient ou définit le PID secondaire d'un champ personnalisé. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype) { get; set; } | Obtient ou définit le type de calcul de la valeur de l'attribut personnalisé pour les lignes récapitulatives. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef) { get; set; } | Obtient ou définit une valeur indiquant si un champ personnalisé est défini par l'utilisateur. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist) { get; } | Obtient la liste&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder) { get; set; } | Obtient ou définit la manière dont les listes de valeurs sont triées. Les valeurs sont : 0=Descendant, 1=Croissant. |

## Méthodes

| Nom | La description |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Méthode d'usine qui crée une définition d'attribut étendue avec recherche. Elle a[`CalculationType`](./calculationtype) est égal àLookup et ne peut être utilisé que dans les ressources. Vous devez spécifier*fieldId* et*alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID de champ. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Méthode d'usine qui crée une définition d'attribut étendue avec recherche. Elle a[`CalculationType`](./calculationtype) est égal àLookup et ne peut être utilisé que dans les ressources. Vous devez spécifier*customFieldType* ,*fieldId* et*alias* lors de l'appel de cette méthode. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Méthode d'usine qui crée une définition d'attribut étendue avec recherche. Elle a[`CalculationType`](./calculationtype) est égal àLookup et ne peut être utilisé que dans les tâches. Vous devez spécifier*fieldId* et*alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID de champ. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Méthode d'usine qui crée une définition d'attribut étendue avec recherche. Elle a[`CalculationType`](./calculationtype) est égal àLookup et ne peut être utilisé que dans les tâches. Vous devez spécifier*customFieldType* ,*fieldId* et*alias* lors de l'appel de cette méthode. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition_1)(ExtendedAttributeResource, string) | Méthode d'usine qui crée une simple définition d'attribut étendu, que Microsoft Project affiche comme "Aucun". Il a[`CalculationType`](./calculationtype) est égal àNone et peut être utilisé dans la ressource uniquement. Vous devez spécifier*fieldId* et*alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID de champ. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Méthode d'usine qui crée une simple définition d'attribut étendu, que Microsoft Project affiche comme "Aucun". Il a[`CalculationType`](./calculationtype) est égal àNone et peut être utilisé dans la ressource uniquement. Vous devez spécifier*customFieldType* ,*fieldId* et*alias* lors de l'appel de cette méthode. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition_1)(ExtendedAttributeTask, string) | Méthode d'usine qui crée une simple définition d'attribut étendu, que Microsoft Project affiche comme "Aucun". Il a[`CalculationType`](./calculationtype) est égal àNone et ne peut être utilisé que dans les tâches. Vous devez spécifier*fieldId* et*alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID de champ. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Méthode d'usine qui crée une simple définition d'attribut étendu, que Microsoft Project affiche comme "Aucun". Il a[`CalculationType`](./calculationtype) est égal àNone et ne peut être utilisé que dans les tâches. Vous devez spécifier*customFieldType* ,*fieldId* et*alias* lors de l'appel de cette méthode. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue)(Value) | Ajoute une valeur à la liste de recherche interne. C'est un moyen préférable pour les manipulations avec le[`ValueList`](./valuelist) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute)() | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur d'ID de champ de cet objet. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_3)(bool) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur d'ID de champ de cet objet et à la valeur d'indicateur spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_4)(DateTime) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur d'ID de champ de cet objet et à la valeur de date spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_5)(decimal) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur d'ID de champ de cet objet et à la valeur numérique spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_1)(Duration) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur d'ID de champ de cet objet et à la valeur de durée spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_6)(string) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur d'ID de champ de cet objet et à la valeur de texte spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_2)(Value) | Crée un nouvel attribut étendu lié avec spécifié[`Value`](../value) article. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals)(object) | Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode)() | Renvoie un code de hachage pour l'instance du[`ExtendedAttributeDefinition`](../extendedattributedefinition) classe. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue)(Value) | Supprime une valeur de la liste de recherche interne. C'est un moyen préférable pour les manipulations avec le[`ValueList`](./valuelist) . |

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks)
* Assemblée [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
