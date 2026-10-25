---
title: "ExtendedAttributeDefinition.Formula"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttributeDefinition. تحصل أو تعين الصيغة التي يستخدمها Microsoft Project لملء حقل مهمة مخصص."
type: docs
weight: 150
url: /ar/net/aspose.tasks/extendedattributedefinition/formula/
---
## ExtendedAttributeDefinition.Formula property

يحصل أو يضبط الصيغة التي يستخدمها Microsoft Project لملء حقل مهمة مخصص.

```csharp
public string Formula { get; set; }
```

## الأمثلة

يوضح كيفية استخدام الدوال المنطقية مع الخصائص الموسعة.

```csharp
var project = CreateTestProjectWithCustomField4();

// تعيين صيغة للخاصية الموسعة
project.ExtendedAttributes[0].Formula = "[Critical]-[Marked]+4+[Active]-Not [Active]";

// طباعة قيمة الخاصية الموسعة
var task = project.RootTask.Children.GetById(1);
Console.WriteLine("Formula with boolean values: " + task.ExtendedAttributes[0].TextValue);
```

يوضح كيفية استخدام دوال الخصائص الموسعة باستخدام حقول أرقام المهام.

```csharp
var project = CreateTestProjectWithCustomField6();

// تعيين صيغة
var attr = project.ExtendedAttributes[0];
attr.Alias = "Task number fields";
attr.Formula = "([Outline Level] + [Priority] + [% Complete])/2";

var task = project.RootTask.Children.GetById(1);

// طباعة قيمة الخاصية الموسعة قبل وبعد تحديث نسبة إكمال المهمة
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
task.Set(Tsk.PercentComplete, 50);
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
```

يوضح كيفية استخدام صيغ الخصائص الموسعة مع الأسماء المستعارة.

```csharp
var project = new Project(DataDir + "Project1.mpp");
project.Set(Prj.NewTasksAreManual, false);

// إنشاء حقل مخصص جديد (Task Text1) مع صيغة ستضاعف تكلفة المهمة
var attr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom");
attr.Alias = "Double Costs";
attr.Formula = "[Cost]*2";
project.ExtendedAttributes.Add(attr);

// إضافة مهمة
var task = project.RootTask.Children.Add("Task");

// تعيين تكلفة المهمة            
task.Set(Tsk.Cost, 100);

project.Save(OutDir + "WriteFormulasInExtendedAttributesToMPP_out.mpp", SaveFileFormat.Mpp);
```

يوضح كيفية استخدام الدوال الرياضية المتعالية مع السمات الموسعة.

```csharp
public void CalculateMathExpressions()
{
    var project = CreateTestProjectWithCustomField2();

    // تعيين الصيغة Sin(pi/2)
    project.ExtendedAttributes[0].Formula = "Sin(3.1415926/2)";

    // طباعة القيمة المحسوبة
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

يوضح كيفية استخدام الدوال الحسابية مع السمات الموسعة.

```csharp
var project = CreateTestProjectWithCustomField5();

    // تعيين صيغة حسابية للخاصية الموسعة
    var attr = project.ExtendedAttributes[0];
    attr.Alias = "Arithmetic Expression";
    attr.Formula = "(1+3*(2+ -5)+8/2)^3";

    // عرض قيمة السمة الموسعة
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

يوضح كيفية استخدام دوال السمة الموسعة عبر حقول المشروع.

```csharp
public void FormulaWithProjectFields()
{
    var project = CreateTestProjectWithCustomFieldWithoutResource();

    // تعيين صيغة
    project.ExtendedAttributes[0].Formula = "\"Total tasks: \" & [Task Count] & \" Total resources: \" & [Resource Count]";

    // طباعة ما إذا كانت قيمة الصيغة محسوبة بشكل صحيح
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

يوضح كيفية استخدام دوال النص مع السمات الموسعة.

```csharp
public static void EvaluateStrConv()
{
    var project = CreateTestProjectWithCustomField3();
    var task = project.RootTask.Children.GetById(1);

    // تعيين الصيغ وطباعة قيمة السمة الموسعة
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

    // تعيين الصيغ وطباعة قيمة السمة الموسعة
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

يوضح كيفية استخدام دوال السمة الموسعة عبر حقول المهمة و/أو الموارد.

```csharp
public void UsingTasksAndResourceFieldsInFormulaCalculations()
{
    try
    {
        var project = CreateTestProjectWithCustomField7();
        var task = project.RootTask.Children.GetById(1);

        // تعيين صيغة للخاصية الموسعة
        var extendedAttributeDefinition1 = project.ExtendedAttributes[0];
        extendedAttributeDefinition1.Alias = "Days from finish to deadline";
        extendedAttributeDefinition1.Formula = "[Deadline] - [Finish]";

        // تعيين موعد نهائي للمهمة وحفظ المشروع
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

// طريقة مساعدة لإنشاء المشروع
public static Project CreateTestProjectWithCustomField7()
{
    var project = new Project(DataDir + "Blank2010.mpp");
    project.Set(Prj.StartDate, new DateTime(2015, 3, 6, 8, 0, 0));

    // إضافة مهمة جديدة مع سمة موسعة
    var task = project.RootTask.Children.Add("Task");
    var extendedAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text5, "My Ext Attr");
    project.ExtendedAttributes.Add(extendedAttributeDefinition);
    var extendedAttribute = extendedAttributeDefinition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(extendedAttribute);

    // إضافة مورد وتعيين المورد
    var rsc = project.Resources.Add("Rsc");
    project.ResourceAssignments.Add(task, rsc);
    return project;
}
```

يوضح كيفية استخدام الدوال الرياضية الشائعة مع السمات الموسعة.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // تعيين الصيغة
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // طباعة قيمة السمة الموسعة
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
        // تعيين الصيغة
        project.ExtendedAttributes[0].Formula = numericFormula;

        // طباعة قيمة السمة الموسعة
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // تعيين الصيغة
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // طباعة قيمة السمة الموسعة
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

### انظر أيضًا

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


