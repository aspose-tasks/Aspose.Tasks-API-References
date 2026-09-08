---
title: "ExtendedAttributeDefinition.Formula"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ExtendedAttributeDefinition. Получает или задает формулу, которую Microsoft Project использует для заполнения пользовательского поля задачи."
type: docs
weight: 150
url: /ru/net/aspose.tasks/extendedattributedefinition/formula/
---
## ExtendedAttributeDefinition.Formula property

Получает или задает формулу, которую Microsoft Project использует для заполнения пользовательского поля задачи.

```csharp
public string Formula { get; set; }
```

## Примеры

Показывает, как использовать булевые функции с расширенными атрибутами.

```csharp
var project = CreateTestProjectWithCustomField4();

// Установить формулу для расширенного атрибута
project.ExtendedAttributes[0].Formula = "[Critical]-[Marked]+4+[Active]-Not [Active]";

// Вывести значение расширенного атрибута
var task = project.RootTask.Children.GetById(1);
Console.WriteLine("Formula with boolean values: " + task.ExtendedAttributes[0].TextValue);
```

Показывает, как использовать функции расширенных атрибутов, используя поля номеров задач.

```csharp
var project = CreateTestProjectWithCustomField6();

// Установить формулу
var attr = project.ExtendedAttributes[0];
attr.Alias = "Task number fields";
attr.Formula = "([Outline Level] + [Priority] + [% Complete])/2";

var task = project.RootTask.Children.GetById(1);

// Вывести значение расширенного атрибута до и после обновления процента выполнения задачи
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
task.Set(Tsk.PercentComplete, 50);
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
```

Показывает, как использовать формулы расширенных атрибутов с псевдонимами.

```csharp
var project = new Project(DataDir + "Project1.mpp");
project.Set(Prj.NewTasksAreManual, false);

// Создать новое пользовательское поле (Task Text1) с формулой, которая удвоит стоимость задачи
var attr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom");
attr.Alias = "Double Costs";
attr.Formula = "[Cost]*2";
project.ExtendedAttributes.Add(attr);

// Добавить задачу
var task = project.RootTask.Children.Add("Task");

// Установить стоимость задачи            
task.Set(Tsk.Cost, 100);

project.Save(OutDir + "WriteFormulasInExtendedAttributesToMPP_out.mpp", SaveFileFormat.Mpp);
```

Показывает, как использовать трансцендентные математические функции с расширенными атрибутами.

```csharp
public void CalculateMathExpressions()
{
    var project = CreateTestProjectWithCustomField2();

    // Установить формулу Sin(pi/2)
    project.ExtendedAttributes[0].Formula = "Sin(3.1415926/2)";

    // Вывести вычисленное значение
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

Показывает, как использовать арифметические функции с расширенными атрибутами.

```csharp
var project = CreateTestProjectWithCustomField5();

    // Установить арифметическую формулу для расширенного атрибута
    var attr = project.ExtendedAttributes[0];
    attr.Alias = "Arithmetic Expression";
    attr.Formula = "(1+3*(2+ -5)+8/2)^3";

    // Отобразить значение расширенного атрибута
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

Показывает, как использовать функции расширенных атрибутов, используя поля проекта.

```csharp
public void FormulaWithProjectFields()
{
    var project = CreateTestProjectWithCustomFieldWithoutResource();

    // Установить формулу
    project.ExtendedAttributes[0].Formula = "\"Total tasks: \" & [Task Count] & \" Total resources: \" & [Resource Count]";

    // Вывести, если значение формулы вычислено правильно
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

Показывает, как использовать текстовые функции с расширенными атрибутами.

```csharp
public static void EvaluateStrConv()
{
    var project = CreateTestProjectWithCustomField3();
    var task = project.RootTask.Children.GetById(1);

    // Установить формулы и вывести значение расширенного атрибута
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

    // Установить формулы и вывести значение расширенного атрибута
    project.ExtendedAttributes[0].Formula = "String(5, 40)";
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    project.ExtendedAttributes[0].Formula = "String(5, \"A\")";
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    project.ExtendedAttributes[0].Formula = "String(-5, \"A\")";

    // #Error
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

Показывает, как использовать функции расширенных атрибутов, используя поля задачи и/или ресурса.

```csharp
public void UsingTasksAndResourceFieldsInFormulaCalculations()
{
    try
    {
        var project = CreateTestProjectWithCustomField7();
        var task = project.RootTask.Children.GetById(1);

        // Установить формулу для расширенного атрибута
        var extendedAttributeDefinition1 = project.ExtendedAttributes[0];
        extendedAttributeDefinition1.Alias = "Days from finish to deadline";
        extendedAttributeDefinition1.Formula = "[Deadline] - [Finish]";

        // Установить срок задачи и сохранить проект
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

// Вспомогательный метод для создания проекта
public static Project CreateTestProjectWithCustomField7()
{
    var project = new Project(DataDir + "Blank2010.mpp");
    project.Set(Prj.StartDate, new DateTime(2015, 3, 6, 8, 0, 0));

    // Добавить новую задачу с расширенным атрибутом
    var task = project.RootTask.Children.Add("Task");
    var extendedAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text5, "My Ext Attr");
    project.ExtendedAttributes.Add(extendedAttributeDefinition);
    var extendedAttribute = extendedAttributeDefinition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(extendedAttribute);

    // Добавить ресурс и назначение ресурса
    var rsc = project.Resources.Add("Rsc");
    project.ResourceAssignments.Add(task, rsc);
    return project;
}
```

Показывает, как использовать общие математические функции с расширенными атрибутами.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Установить формулу
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Вывести значение расширенного атрибута
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
        // Установить формулу
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Вывести значение расширенного атрибута
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Установить формулу
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Вывести значение расширенного атрибута
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

### См. также

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


