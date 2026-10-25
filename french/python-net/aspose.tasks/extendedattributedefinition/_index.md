---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 310
url: /fr/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Représente une définition d'attribut étendu associée à un projet.

Le type ExtendedAttributeDefinition expose les membres suivants :
## Propriétés
| Nom | Description |
| :- | :- |
| field_id | Obtient ou définit la correspondance à l'ID du projet d'un champ personnalisé.<br/>            Utilisez la représentation sous forme de chaîne d'une constante de la classe [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) pour spécifier la propriété [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| field_name | Obtient le nom d'un champ personnalisé. |
| cf_type | Obtient le type d'un champ personnalisé. |
| guid | Obtient ou définit le GUID d'un champ personnalisé. |
| element_type | Obtient ou définit l'attribut étendu associé<br/>            à une tâche, une ressource ou une affectation. |
| max_multi_values | Obtient ou définit le nombre maximal de valeurs que vous pouvez définir dans une liste déroulante. |
| user_def | Obtient ou définit une valeur indiquant si un champ personnalisé est défini par l'utilisateur. |
| alias | Obtient ou définit l'alias d'un champ personnalisé. |
| secondary_pid | Obtient ou définit le PID secondaire d'un champ personnalisé. |
| auto_roll_down | Obtient ou définit une valeur indiquant si le déroulement automatique vers les affectations est activé. |
| default_guid | Obtient ou définit le GUID de l'entrée de la table de recherche par défaut. |
| lookup_uid | Obtient un GUID de la table de recherche associée à un champ personnalisé. |
| phonetics_alias | Obtient ou définit la prononciation phonétique de l'alias d'un champ personnalisé. |
| rollup_type | Obtient ou définit la manière dont les rollups sont calculés. |
| calculation_type | Obtient ou définit le type de calcul de la valeur de l'attribut personnalisé. |
| summary_rows_calculation_type | Obtient ou définit le type de calcul de la valeur de l'attribut personnalisé pour les lignes de synthèse. |
| formula | Obtient ou définit la formule que Microsoft Project utilise pour remplir un champ de tâche personnalisé. |
| graphical_indicator | Obtient ou définit les informations des indicateurs graphiques associées à l'attribut étendu.<br/>            Applicable au format MPP. |
| restrict_values | Obtient ou définit une valeur indiquant si les valeurs des champs personnalisés sont limitées aux valeurs de la [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| valuelist_sort_order | Obtient ou définit la façon dont les listes de valeurs sont triées. Les valeurs sont : 0=Descendant, 1=Ascendant. |
| append_new_values | Obtient ou définit une valeur indiquant si les nouvelles valeurs ajoutées à un projet sont automatiquement ajoutées à la liste. |
| default | Obtient ou définit la valeur par défaut dans la liste. |
| value_list | Obtient la List<Value> ValueList. |
| secondary_guid | Obtient ou définit le guid secondaire de l'attribut étendu. |
| parent_project | Obtient le projet parent de l'instance [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
## Méthodes
| Nom | Description |
| :- | :- |
| create_extended_attribute() | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet. |
| create_extended_attribute(text_value) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur texte spécifiée. |
| create_extended_attribute(numeric_value) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur numérique spécifiée. |
| create_extended_attribute(date_time_value) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de date spécifiée. |
| create_extended_attribute(duration_value) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de durée spécifiée. |
| create_extended_attribute(flag_value) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de drapeau spécifiée. |
| create_extended_attribute(lookup_value) | Crée un nouvel attribut étendu lié à l'élément [Value](/tasks/python-net/aspose.tasks/value/) spécifié. |
| create_task_definition(custom_field_type, field_id, alias) | Méthode d'usine qui crée une définition d'attribut étendu simple, affichée par Microsoft Project comme \"None\".<br/>            Elle possède [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) égal à [NONE](/tasks/python-net/aspose.tasks/calculationtype/) et ne peut être utilisée que dans les Tâches.<br/>            Vous devez spécifier |
| create_task_definition(field_id, alias) | Méthode d'usine qui crée une définition d'attribut étendu simple, affichée par Microsoft Project comme \"None\".<br/>            Elle possède [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) égal à [NONE](/tasks/python-net/aspose.tasks/calculationtype/) et ne peut être utilisée que dans les Tâches.<br/>            Vous devez spécifier |
| create_resource_definition(custom_field_type, field_id, alias) | Méthode d'usine qui crée une définition d'attribut étendu simple, affichée par Microsoft Project comme \"None\".<br/>            Elle possède [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) égal à [NONE](/tasks/python-net/aspose.tasks/calculationtype/) et ne peut être utilisée que dans les Ressources.<br/>            Vous devez spécifier |
| create_resource_definition(field_id, alias) | Méthode d'usine qui crée une définition d'attribut étendu simple, affichée par Microsoft Project comme \"None\".<br/>            Elle possède [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) égal à [NONE](/tasks/python-net/aspose.tasks/calculationtype/) et ne peut être utilisée que dans les Ressources.<br/>            Vous devez spécifier |
| create_lookup_task_definition(field_id, alias) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche.<br/>            Elle possède [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) égal à [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) et ne peut être utilisée que dans les Tâches.<br/>            Vous devez spécifier |
| create_lookup_task_definition(custom_field_type, field_id, alias) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche.<br/>            Elle possède [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) égal à [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) et ne peut être utilisée que dans les Tâches.<br/>            Vous devez spécifier |
| create_lookup_resource_definition(field_id, alias) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche.<br/>            Elle possède [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) égal à [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) et ne peut être utilisée que dans les Ressources.<br/>            Vous devez spécifier |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche.<br/>            Elle possède [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) égal à [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) et ne peut être utilisée que dans les Ressources.<br/>            Vous devez spécifier |
| add_lookup_value(value) | Ajoute une valeur à la liste de recherche interne. C'est une méthode préférée pour manipuler la [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| remove_lookup_value(value) | Supprime une valeur de la liste de recherche interne. C'est une méthode préférée pour manipuler la [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |

### Voir aussi

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

