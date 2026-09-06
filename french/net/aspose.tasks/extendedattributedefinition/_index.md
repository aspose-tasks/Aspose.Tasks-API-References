---
title: "Classe ExtendedAttributeDefinition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ExtendedAttributeDefinition. Représente une définition d’attribut étendu associée à un projet"
type: docs
weight: 540
url: /fr/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Représente une définition d'attribut étendu associée à un projet.

```csharp
public class ExtendedAttributeDefinition
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Obtient ou définit l’alias d’un champ personnalisé. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Obtient ou définit une valeur indiquant si les nouvelles valeurs ajoutées à un projet sont automatiquement ajoutées à la liste. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Obtient ou définit une valeur indiquant si un déploiement automatique vers les affectations est activé. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Obtient ou définit le type de calcul de la valeur de l’attribut personnalisé. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Obtient le type d’un champ personnalisé. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Obtient ou définit la valeur par défaut dans la liste. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Obtient ou définit le GUID de l’entrée du tableau de recherche par défaut. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Obtient ou définit si l’attribut étendu est associé à une tâche, une ressource ou une affectation. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Obtient ou définit la correspondance à l’identifiant de projet d’un champ personnalisé. Utilisez la représentation sous forme de chaîne d’une constante de la classe [`ExtendedAttributeTask`](../extendedattributetask/) pour spécifier la propriété [`FieldId`](./fieldid/). |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Obtient le nom d'un champ personnalisé. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Obtient ou définit la formule que Microsoft Project utilise pour remplir un champ de tâche personnalisé. |
| [GraphicalIndicator](../../aspose.tasks/extendedattributedefinition/graphicalindicator/) { get; set; } | Obtient ou définit les informations d'indicateurs graphiques associées à l'attribut étendu. Applicable au format MPP. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Obtient ou définit le GUID d'un champ personnalisé. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Obtient le GUID de la table de recherche associée à un champ personnalisé. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Obtient ou définit le nombre maximal de valeurs que vous pouvez définir dans une liste déroulante. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | Obtient le projet parent pour l'instance `ExtendedAttributeDefinition`. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Obtient ou définit la prononciation phonétique de l'alias d'un champ personnalisé. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Obtient ou définit une valeur indiquant si les valeurs du champ personnalisé sont limitées aux valeurs de la [`ValueList`](./valuelist/). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Obtient ou définit la manière dont les totaux sont calculés. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Obtient ou définit le GUID secondaire de l'attribut étendu. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Obtient ou définit le PID secondaire d'un champ personnalisé. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Obtient ou définit le type de calcul de la valeur de l'attribut personnalisé pour les lignes de synthèse. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Obtient ou définit une valeur indiquant si un champ personnalisé est défini par l'utilisateur. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | Obtient la List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Obtient ou définit la façon dont les listes de valeurs sont triées. Les valeurs sont : 0=Descendant, 1=Ascendant. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle possède [`CalculationType`](./calculationtype/) égal à Lookup et ne peut être utilisée que dans les Ressources. Vous devez spécifier *fieldId* et *alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID du champ. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle possède [`CalculationType`](./calculationtype/) égal à Lookup et ne peut être utilisée que dans les Ressources. Vous devez spécifier *customFieldType*, *fieldId* et *alias* lors de l'appel de cette méthode. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle possède [`CalculationType`](./calculationtype/) égal à Lookup et ne peut être utilisée que dans les Tâches. Vous devez spécifier *fieldId* et *alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID du champ. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle possède [`CalculationType`](./calculationtype/) égal à Lookup et ne peut être utilisée que dans les Tâches. Vous devez spécifier *customFieldType*, *fieldId* et *alias* lors de l'appel de cette méthode. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme « None ». Elle possède [`CalculationType`](./calculationtype/) égal à None et ne peut être utilisée que dans les Ressources. Vous devez spécifier *fieldId* et *alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID du champ. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme « None ». Elle possède [`CalculationType`](./calculationtype/) égal à None et ne peut être utilisée que dans les Ressources. Vous devez spécifier *customFieldType*, *fieldId* et *alias* lors de l'appel de cette méthode. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme « None ». Elle possède [`CalculationType`](./calculationtype/) égal à None et ne peut être utilisée que dans les Tâches. Vous devez spécifier *fieldId* et *alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID du champ. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme « None ». Elle possède [`CalculationType`](./calculationtype/) égal à None et ne peut être utilisée que dans les Tâches. Vous devez spécifier *customFieldType*, *fieldId* et *alias* lors de l'appel de cette méthode. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Ajoute une valeur à la liste de recherche interne. C'est une méthode préférée pour manipuler la [`ValueList`](./valuelist/). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de drapeau spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de date spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur numérique spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de durée spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de texte spécifiée. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Crée un nouvel attribut étendu lié à l'élément [`Value`](../value/) spécifié. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Renvoie un code de hachage pour l'instance de la classe `ExtendedAttributeDefinition`. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Supprime une valeur de la liste de recherche interne. C'est une méthode préférée pour les manipulations avec le [`ValueList`](./valuelist/). |

## Exemples

Montre comment utiliser les fonctions mathématiques courantes avec les attributs étendus.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Définir la formule
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Imprimer la valeur de l'attribut étendu
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static void EvaluateIsNumeric()
{
    string[] numericFormulas =
        {
            "IsNumeric('AAA')", @"IsNUmeric(1)", "IsNumeric(1<0)", "IsNumeric(\"1.1\")", "IsNumeric(Choose((2 + Sgn(2^-3)), 123, \"one two three\"))"
        };

    var project = CreateTestProjectWithCustomField();

    foreach (var numericFormula in numericFormulas)
    {
        // Définir la formule
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Imprimer la valeur de l'attribut étendu
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Définir la formule
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Imprimer la valeur de l'attribut étendu
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static Project CreateTestProjectWithCustomField()
{
    var project = new Project();
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom Field");
    project.ExtendedAttributes.Add(definition);

    var task = project.RootTask.Children.Add("Task");

    var attribute = definition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


