---
title: "Aspose::Tasks::ExtendedAttributeDefinition classe"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks pour C++"
description: "Représente une définition d'attribut étendu associée à un projet."
type: docs
weight: 10
url: /fr/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Représente une définition d'attribut étendu associée à un projet.

## Méthodes

| Nom | Description |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | Ajoute une valeur à la liste de recherche interne. C’est une méthode préférable pour les manipulations avec la ValueList . |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet. |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle a CalculationType égal à Tasks::CalculationType::Lookup et ne peut être utilisée que dans Resources. Vous devez spécifier customFieldType , fieldId et alias lors de l'appel de cette méthode. |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle a CalculationType égal à Tasks::CalculationType::Lookup et ne peut être utilisée que dans Tasks. Vous devez spécifier customFieldType , fieldId et alias lors de l'appel de cette méthode. |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle a CalculationType égal à Tasks::CalculationType::None et ne peut être utilisée que dans Resource. Vous devez spécifier customFieldType , fieldId et alias lors de l'appel de cette méthode. |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle a CalculationType égal à Tasks::CalculationType::None et ne peut être utilisée que dans Tasks. Vous devez spécifier customFieldType , fieldId et alias lors de l'appel de cette méthode. |
| [Equals](./equals/) | Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié. |
| [get_Alias](./get_alias/) | Obtient l'alias d'un champ personnalisé. |
| [get_AppendNewValues](./get_appendnewvalues/) | Obtient une valeur indiquant si les nouvelles valeurs ajoutées à un projet sont automatiquement ajoutées à la liste. |
| [get_AutoRollDown](./get_autorolldown/) | Obtient une valeur indiquant si un roulement automatique vers les affectations est activé. |
| [get_CalculationType](./get_calculationtype/) | Obtient le type de calcul de la valeur de l'attribut personnalisé. |
| [get_CfType](./get_cftype/) | Obtient le type d'un champ personnalisé. |
| [get_Default](./get_default/) | Obtient la valeur par défaut dans la liste. |
| [get_DefaultGuid](./get_defaultguid/) | Obtient le Guid de l'entrée de la table de recherche par défaut. |
| [get_ElementType](./get_elementtype/) | Obtient l'attribut étendu associé à une tâche, une ressource ou une affectation. |
| [get_FieldId](./get_fieldid/) | Obtient correspond à l'ID du projet d'un champ personnalisé. Utilisez la représentation sous forme de chaîne d'une constante de la classe Aspose::Tasks::ExtendedAttributeTask pour spécifier la propriété FieldId. |
| [get_FieldName](./get_fieldname/) | Obtient le nom d'un champ personnalisé. |
| [get_Formula](./get_formula/) | Obtient la formule que Microsoft Project utilise pour remplir un champ de tâche personnalisé. |
| [get_GraphicalIndicator](./get_graphicalindicator/) | Obtient les informations des indicateurs graphiques associées à l'attribut étendu. Applicable au format MPP. |
| [get_Guid](./get_guid/) | Obtient le Guid d'un champ personnalisé. |
| [get_LookupUid](./get_lookupuid/) | Obtient un Guid de la table de recherche associée à un champ personnalisé. |
| [get_MaxMultiValues](./get_maxmultivalues/) | Obtient le nombre maximal de valeurs que vous pouvez définir dans une liste de sélection. |
| [get_ParentProject](./get_parentproject/) | Obtient le projet parent de l'instance ExtendedAttributeDefinition. |
| [get_PhoneticsAlias](./get_phoneticsalias/) | Obtient la prononciation phonétique de l'alias d'un champ personnalisé. |
| [get_RestrictValues](./get_restrictvalues/) | Obtient une valeur indiquant si les valeurs du champ personnalisé sont limitées aux valeurs de la ValueList. |
| [get_RollupType](./get_rolluptype/) | Obtient la manière dont les rollups sont calculés. |
| [get_SecondaryGuid](./get_secondaryguid/) | Obtient le guid secondaire de l'attribut étendu. |
| [get_SecondaryPid](./get_secondarypid/) | Obtient le PID secondaire d'un champ personnalisé. |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | Obtient le type de calcul de la valeur de l'attribut personnalisé pour les lignes de synthèse. |
| [get_UserDef](./get_userdef/) | Obtient une valeur indiquant si un champ personnalisé est défini par l'utilisateur. |
| [get_ValueList](./get_valuelist/) | Obtient la List< Value > ValueList. |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | Obtient la manière dont les listes de valeurs sont triées. Les valeurs sont : 0=Descendant, 1=Ascendant. |
| [GetHashCode](./gethashcode/) | Renvoie un code de hachage pour l'instance de la classe ExtendedAttributeDefinition. |
| [RemoveLookupValue](./removelookupvalue/) | Supprime une valeur de la liste de recherche interne. C’est une méthode préférable pour les manipulations avec la ValueList. |
| [set_Alias](./set_alias/) | Définit l'alias d'un champ personnalisé. |
| [set_AppendNewValues](./set_appendnewvalues/) | Définit une valeur indiquant si les nouvelles valeurs ajoutées à un projet sont automatiquement ajoutées à la liste. |
| [set_AutoRollDown](./set_autorolldown/) | Définit une valeur indiquant si un déploiement automatique vers les affectations est activé. |
| [set_CalculationType](./set_calculationtype/) | Définit le type de calcul de la valeur de l'attribut personnalisé. |
| [set_Default](./set_default/) | Définit la valeur par défaut dans la liste. |
| [set_DefaultGuid](./set_defaultguid/) | Définit le Guid de l'entrée de la table de recherche par défaut. |
| [set_ElementType](./set_elementtype/) | Définit que l'attribut étendu est associé à une tâche, une ressource ou une affectation. |
| [set_FieldId](./set_fieldid/) | Définit correspond à l'identifiant du projet d'un champ personnalisé. Utilisez la représentation sous forme de chaîne d'une constante de la classe Aspose::Tasks::ExtendedAttributeTask pour spécifier la propriété FieldId. |
| [set_Formula](./set_formula/) | Définit la formule que Microsoft Project utilise pour remplir un champ de tâche personnalisé. |
| [set_GraphicalIndicator](./set_graphicalindicator/) | Définit les informations d'indicateurs graphiques associées à l'attribut étendu. Applicable au format MPP. |
| [set_Guid](./set_guid/) | Définit le Guid d'un champ personnalisé. |
| [set_MaxMultiValues](./set_maxmultivalues/) | Définit le nombre maximal de valeurs que vous pouvez définir dans une liste déroulante. |
| [set_PhoneticsAlias](./set_phoneticsalias/) | Définit la prononciation phonétique de l'alias d'un champ personnalisé. |
| [set_RestrictValues](./set_restrictvalues/) | Définit une valeur indiquant si les valeurs du champ personnalisé sont limitées aux valeurs de la ValueList. |
| [set_RollupType](./set_rolluptype/) | Définit la façon dont les agrégations sont calculées. |
| [set_SecondaryGuid](./set_secondaryguid/) | Définit le guid secondaire de l'attribut étendu. |
| [set_SecondaryPid](./set_secondarypid/) | Définit le PID secondaire d'un champ personnalisé. |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | Définit le type de calcul de la valeur de l'attribut personnalisé pour les lignes de synthèse. |
| [set_UserDef](./set_userdef/) | Définit une valeur indiquant si un champ personnalisé est défini par l'utilisateur. |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | Définit la façon dont les listes de valeurs sont triées. Les valeurs sont : 0=Descendant, 1=Ascendant. |

