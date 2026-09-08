---
title: "ExtendedAttributeDefinition.Formula"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition eigenschap. Haalt of stelt de formule in die Microsoft Project gebruikt om een aangepast taakveld te vullen."
type: docs
weight: 150
url: /nl/net/aspose.tasks/extendedattributedefinition/formula/
---
## ExtendedAttributeDefinition.Formula property

Haalt de formule op of stelt deze in die Microsoft Project gebruikt om een aangepast taakveld te vullen.

```csharp
public string Formula { get; set; }
```

## Voorbeelden

Toont hoe booleaanse functies te gebruiken met uitgebreide attributen.

```csharp
var project = CreateTestProjectWithCustomField4();

// Formule instellen voor uitgebreid attribuut
project.ExtendedAttributes[0].Formula = "[Critical]-[Marked]+4+[Active]-Not [Active]";

// Waarde van uitgebreid attribuut afdrukken
var task = project.RootTask.Children.GetById(1);
Console.WriteLine("Formula with boolean values: " + task.ExtendedAttributes[0].TextValue);
```

Toont hoe functies van uitgebreide attributen te gebruiken via taaknummer‑velden.

```csharp
var project = CreateTestProjectWithCustomField6();

// Formule instellen
var attr = project.ExtendedAttributes[0];
attr.Alias = "Task number fields";
attr.Formula = "([Outline Level] + [Priority] + [% Complete])/2";

var task = project.RootTask.Children.GetById(1);

// Waarde van uitgebreid attribuut afdrukken vóór en na het bijwerken van de taakvoltooiingspercentage
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
task.Set(Tsk.PercentComplete, 50);
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
```

Toont hoe formules van uitgebreide attributen te gebruiken met aliassen.

```csharp
var project = new Project(DataDir + "Project1.mpp");
project.Set(Prj.NewTasksAreManual, false);

// Maak een nieuw aangepast veld (Task Text1) met een formule die de taakkosten verdubbelt
var attr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom");
attr.Alias = "Double Costs";
attr.Formula = "[Cost]*2";
project.ExtendedAttributes.Add(attr);

// Voeg een taak toe
var task = project.RootTask.Children.Add("Task");

// Stel taakkosten in            
task.Set(Tsk.Cost, 100);

project.Save(OutDir + "WriteFormulasInExtendedAttributesToMPP_out.mpp", SaveFileFormat.Mpp);
```

Toont hoe transcendente wiskundige functies te gebruiken met uitgebreide attributen.

```csharp
public void CalculateMathExpressions()
{
    var project = CreateTestProjectWithCustomField2();

    // Stel formule Sin(pi/2) in
    project.ExtendedAttributes[0].Formula = "Sin(3.1415926/2)";

    // Print berekende waarde
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

Toont hoe rekenkundige functies te gebruiken met uitgebreide attributen.

```csharp
var project = CreateTestProjectWithCustomField5();

    // Stel rekenkundige formule in voor uitgebreid attribuut
    var attr = project.ExtendedAttributes[0];
    attr.Alias = "Arithmetic Expression";
    attr.Formula = "(1+3*(2+ -5)+8/2)^3";

    // Toon waarde van uitgebreid attribuut
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

Toont hoe uitgebreide attribuutfuncties te gebruiken via projectvelden.

```csharp
public void FormulaWithProjectFields()
{
    var project = CreateTestProjectWithCustomFieldWithoutResource();

    // Formule instellen
    project.ExtendedAttributes[0].Formula = "\"Total tasks: \" & [Task Count] & \" Total resources: \" & [Resource Count]";

    // Print of de formulewaarde correct is berekend
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

Toont hoe tekstfuncties te gebruiken met uitgebreide attributen.

```csharp
public static void EvaluateStrConv()
{
    var project = CreateTestProjectWithCustomField3();
    var task = project.RootTask.Children.GetById(1);

    // Stel formules in en print de waarde van het uitgebreide attribuut
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

    // Stel formules in en print de waarde van het uitgebreide attribuut
    project.ExtendedAttributes[0].Formula = "String(5, 40)";
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    project.ExtendedAttributes[0].Formula = "String(5, \"A\")";
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    project.ExtendedAttributes[0].Formula = "String(-5, \"A\")";

    // #Fout
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

Toont hoe uitgebreide attribuutfuncties te gebruiken via taak- en/of resourcevelden.

```csharp
public void UsingTasksAndResourceFieldsInFormulaCalculations()
{
    try
    {
        var project = CreateTestProjectWithCustomField7();
        var task = project.RootTask.Children.GetById(1);

        // Formule instellen voor uitgebreid attribuut
        var extendedAttributeDefinition1 = project.ExtendedAttributes[0];
        extendedAttributeDefinition1.Alias = "Days from finish to deadline";
        extendedAttributeDefinition1.Formula = "[Deadline] - [Finish]";

        // Stel taakdeadline in en sla project op
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

// Helper-methode om een project te maken
public static Project CreateTestProjectWithCustomField7()
{
    var project = new Project(DataDir + "Blank2010.mpp");
    project.Set(Prj.StartDate, new DateTime(2015, 3, 6, 8, 0, 0));

    // Voeg nieuwe taak toe met uitgebreid attribuut
    var task = project.RootTask.Children.Add("Task");
    var extendedAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text5, "My Ext Attr");
    project.ExtendedAttributes.Add(extendedAttributeDefinition);
    var extendedAttribute = extendedAttributeDefinition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(extendedAttribute);

    // Voeg resource en resource-toewijzing toe
    var rsc = project.Resources.Add("Rsc");
    project.ResourceAssignments.Add(task, rsc);
    return project;
}
```

Toont hoe je algemene wiskundige functies gebruikt met uitgebreide attributen.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Formule instellen
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Print uitgebreide attribuutwaarde
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
        // Formule instellen
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Print uitgebreide attribuutwaarde
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Formule instellen
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Print uitgebreide attribuutwaarde
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

### Zie ook

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


