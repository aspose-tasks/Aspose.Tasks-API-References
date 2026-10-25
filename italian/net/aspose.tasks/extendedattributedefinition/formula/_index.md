---
title: "ExtendedAttributeDefinition.Formula"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ExtendedAttributeDefinition. Ottiene o imposta la formula che Microsoft Project utilizza per popolare un campo personalizzato del compito."
type: docs
weight: 150
url: /it/net/aspose.tasks/extendedattributedefinition/formula/
---
## ExtendedAttributeDefinition.Formula property

Ottiene o imposta la formula che Microsoft Project utilizza per popolare un campo attività personalizzato.

```csharp
public string Formula { get; set; }
```

## Esempi

Mostra come utilizzare le funzioni booleane con gli attributi estesi.

```csharp
var project = CreateTestProjectWithCustomField4();

// Imposta la formula per l'attributo esteso
project.ExtendedAttributes[0].Formula = "[Critical]-[Marked]+4+[Active]-Not [Active]";

// Stampa il valore dell'attributo esteso
var task = project.RootTask.Children.GetById(1);
Console.WriteLine("Formula with boolean values: " + task.ExtendedAttributes[0].TextValue);
```

Mostra come utilizzare le funzioni degli attributi estesi usando i campi numero del compito.

```csharp
var project = CreateTestProjectWithCustomField6();

// Imposta formula
var attr = project.ExtendedAttributes[0];
attr.Alias = "Task number fields";
attr.Formula = "([Outline Level] + [Priority] + [% Complete])/2";

var task = project.RootTask.Children.GetById(1);

// Stampa il valore dell'attributo esteso prima e dopo l'aggiornamento della percentuale di completamento del compito
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
task.Set(Tsk.PercentComplete, 50);
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
```

Mostra come utilizzare le formule degli attributi estesi con alias.

```csharp
var project = new Project(DataDir + "Project1.mpp");
project.Set(Prj.NewTasksAreManual, false);

// Crea un nuovo campo personalizzato (Task Text1) con formula che raddoppierà il costo dell'attività
var attr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom");
attr.Alias = "Double Costs";
attr.Formula = "[Cost]*2";
project.ExtendedAttributes.Add(attr);

// Aggiungi un'attività
var task = project.RootTask.Children.Add("Task");

// Imposta costo attività            
task.Set(Tsk.Cost, 100);

project.Save(OutDir + "WriteFormulasInExtendedAttributesToMPP_out.mpp", SaveFileFormat.Mpp);
```

Mostra come utilizzare le funzioni matematiche trascendenti con attributi estesi.

```csharp
public void CalculateMathExpressions()
{
    var project = CreateTestProjectWithCustomField2();

    // Imposta formula Sin(pi/2)
    project.ExtendedAttributes[0].Formula = "Sin(3.1415926/2)";

    // Stampa valore calcolato
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine("Sin(pi/2): {0}", task.ExtendedAttributes[0].NumericValue);
}

public static Project CreateTestProjectWithCustomField2()
{
    var project = new Project();
    var attr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number1, "Sine");
    project.ExtendedAttributes.Add(attr);

    var task = project.RootTask.Children.Add("Task");

    var attribute = attr.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

Mostra come utilizzare le funzioni aritmetiche con attributi estesi.

```csharp
var project = CreateTestProjectWithCustomField5();

    // Imposta formula aritmetica per l'attributo esteso
    var attr = project.ExtendedAttributes[0];
    attr.Alias = "Arithmetic Expression";
    attr.Formula = "(1+3*(2+ -5)+8/2)^3";

    // Visualizza valore dell'attributo esteso
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
}

public static Project CreateTestProjectWithCustomField5()
{
    var project = new Project();
    project.Set(Prj.StartDate, new DateTime(2015, 3, 6, 8, 0, 0));
    var attr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number1, "Custom");
    project.ExtendedAttributes.Add(attr);

    var task = project.RootTask.Children.Add("Task");
    var extendedAttribute = attr.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(extendedAttribute);
    return project;
}
```

Mostra come utilizzare le funzioni di attributi estesi usando i campi del progetto.

```csharp
public void FormulaWithProjectFields()
{
    var project = CreateTestProjectWithCustomFieldWithoutResource();

    // Imposta formula
    project.ExtendedAttributes[0].Formula = "\"Total tasks: \" & [Task Count] & \" Total resources: \" & [Resource Count]";

    // Stampa se il valore della formula è calcolato correttamente
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine("Check Total tasks: 1 Total resources: 0 - {0}", task.ExtendedAttributes[0].TextValue.Equals("Total tasks: 1 Total resources: 0"));
}

public static Project CreateTestProjectWithCustomFieldWithoutResource()
{
    var project = new Project();
    project.Set(Prj.StartDate, new DateTime(2015, 3, 6, 8, 0, 0));
    var attr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom");
    project.ExtendedAttributes.Add(attr);

    var task = project.RootTask.Children.Add("Task");
    var attribute = attr.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

Mostra come utilizzare le funzioni di testo con attributi estesi.

```csharp
public static void EvaluateStrConv()
{
    var project = CreateTestProjectWithCustomField3();
    var task = project.RootTask.Children.GetById(1);

    // Imposta formule e stampa il valore dell'attributo esteso
    project.ExtendedAttributes[0].Formula = "StrConv(\"sTring and sTRINg\",3)";
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    project.ExtendedAttributes[0].Formula = "StrConv(\"sTring and sTRINg\",1)";
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    project.ExtendedAttributes[0].Formula = "StrConv(\"sTring and sTRINg\",2)";
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static void EvaluateStringFunction()
{
    var project = CreateTestProjectWithCustomField3();
    var task = project.RootTask.Children.GetById(1);

    // Imposta formule e stampa il valore dell'attributo esteso
    project.ExtendedAttributes[0].Formula = "String(5, 40)";
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    project.ExtendedAttributes[0].Formula = "String(5, \"A\")";
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    project.ExtendedAttributes[0].Formula = "String(-5, \"A\")";

    // #Errore
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static Project CreateTestProjectWithCustomField3()
{
    var project = new Project();
    var attr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom Field");
    project.ExtendedAttributes.Add(attr);

    var task = project.RootTask.Children.Add("Task");

    var attribute = attr.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

Mostra come utilizzare le funzioni di attributi estesi usando i campi delle attività e/o delle risorse.

```csharp
public void UsingTasksAndResourceFieldsInFormulaCalculations()
{
    try
    {
        var project = CreateTestProjectWithCustomField7();
        var task = project.RootTask.Children.GetById(1);

        // Imposta la formula per l'attributo esteso
        var extendedAttributeDefinition1 = project.ExtendedAttributes[0];
        extendedAttributeDefinition1.Alias = "Days from finish to deadline";
        extendedAttributeDefinition1.Formula = "[Deadline] - [Finish]";

        // Imposta scadenza attività e salva il progetto
        task.Set(Tsk.Deadline, new DateTime(2015, 3, 20, 17, 0, 0));
        project.Save(OutDir + "UsingTasksAndResourceFields_out.mpp", SaveFileFormat.Mpp);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

// Metodo di supporto per creare il progetto
public static Project CreateTestProjectWithCustomField7()
{
    var project = new Project(DataDir + "Blank2010.mpp");
    project.Set(Prj.StartDate, new DateTime(2015, 3, 6, 8, 0, 0));

    // Aggiungi nuova attività con attributo esteso
    var task = project.RootTask.Children.Add("Task");
    var extendedAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text5, "My Ext Attr");
    project.ExtendedAttributes.Add(extendedAttributeDefinition);
    var extendedAttribute = extendedAttributeDefinition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(extendedAttribute);

    // Aggiungi risorsa e assegnazione risorsa
    var rsc = project.Resources.Add("Rsc");
    project.ResourceAssignments.Add(task, rsc);
    return project;
}
```

Mostra come utilizzare le funzioni matematiche comuni con gli attributi estesi.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Imposta formula
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Stampa il valore dell'attributo esteso
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
        // Imposta formula
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Stampa il valore dell'attributo esteso
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Imposta formula
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Stampa il valore dell'attributo esteso
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

### Vedi anche

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


