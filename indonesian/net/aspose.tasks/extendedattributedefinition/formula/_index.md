---
title: "ExtendedAttributeDefinition.Formula"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ExtendedAttributeDefinition. Mendapatkan atau mengatur formula yang digunakan Microsoft Project untuk mengisi bidang tugas khusus."
type: docs
weight: 150
url: /id/net/aspose.tasks/extendedattributedefinition/formula/
---
## ExtendedAttributeDefinition.Formula property

Mendapatkan atau mengatur rumus yang Microsoft Project gunakan untuk mengisi bidang tugas khusus.

```csharp
public string Formula { get; set; }
```

## Contoh

Menampilkan cara menggunakan fungsi boolean dengan atribut yang diperluas.

```csharp
var project = CreateTestProjectWithCustomField4();

// Atur formula untuk atribut yang diperluas
project.ExtendedAttributes[0].Formula = "[Critical]-[Marked]+4+[Active]-Not [Active]";

// Cetak nilai atribut yang diperluas
var task = project.RootTask.Children.GetById(1);
Console.WriteLine("Formula with boolean values: " + task.ExtendedAttributes[0].TextValue);
```

Menampilkan cara menggunakan fungsi atribut yang diperluas dengan menggunakan bidang nomor tugas.

```csharp
var project = CreateTestProjectWithCustomField6();

// Atur formula
var attr = project.ExtendedAttributes[0];
attr.Alias = "Task number fields";
attr.Formula = "([Outline Level] + [Priority] + [% Complete])/2";

var task = project.RootTask.Children.GetById(1);

// Cetak nilai atribut yang diperluas sebelum dan sesudah memperbarui persentase penyelesaian tugas
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
task.Set(Tsk.PercentComplete, 50);
Console.WriteLine(task.ExtendedAttributes[0].NumericValue);
```

Menampilkan cara menggunakan formula atribut yang diperluas dengan alias.

```csharp
var project = new Project(DataDir + "Project1.mpp");
project.Set(Prj.NewTasksAreManual, false);

// Buat bidang khusus baru (Task Text1) dengan rumus yang akan menggandakan biaya tugas
var attr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom");
attr.Alias = "Double Costs";
attr.Formula = "[Cost]*2";
project.ExtendedAttributes.Add(attr);

// Tambahkan sebuah tugas
var task = project.RootTask.Children.Add("Task");

// Atur biaya tugas            
task.Set(Tsk.Cost, 100);

project.Save(OutDir + "WriteFormulasInExtendedAttributesToMPP_out.mpp", SaveFileFormat.Mpp);
```

Menampilkan cara menggunakan fungsi matematika transenden dengan atribut tambahan.

```csharp
public void CalculateMathExpressions()
{
    var project = CreateTestProjectWithCustomField2();

    // Atur rumus Sin(pi/2)
    project.ExtendedAttributes[0].Formula = "Sin(3.1415926/2)";

    // Cetak nilai yang dihitung
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

Menampilkan cara menggunakan fungsi aritmetika dengan atribut tambahan.

```csharp
var project = CreateTestProjectWithCustomField5();

    // Atur rumus aritmetika untuk atribut tambahan
    var attr = project.ExtendedAttributes[0];
    attr.Alias = "Arithmetic Expression";
    attr.Formula = "(1+3*(2+ -5)+8/2)^3";

    // Tampilkan nilai atribut tambahan
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

Menampilkan cara menggunakan fungsi atribut tambahan dengan menggunakan bidang proyek.

```csharp
public void FormulaWithProjectFields()
{
    var project = CreateTestProjectWithCustomFieldWithoutResource();

    // Atur formula
    project.ExtendedAttributes[0].Formula = "\"Total tasks: \" & [Task Count] & \" Total resources: \" & [Resource Count]";

    // Cetak jika nilai rumus dihitung dengan benar
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

Menampilkan cara menggunakan fungsi teks dengan atribut tambahan.

```csharp
public static void EvaluateStrConv()
{
    var project = CreateTestProjectWithCustomField3();
    var task = project.RootTask.Children.GetById(1);

    // Atur rumus dan cetak nilai atribut tambahan
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

    // Atur rumus dan cetak nilai atribut tambahan
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

Menampilkan cara menggunakan fungsi atribut tambahan dengan menggunakan bidang tugas dan/atau sumber daya.

```csharp
public void UsingTasksAndResourceFieldsInFormulaCalculations()
{
    try
    {
        var project = CreateTestProjectWithCustomField7();
        var task = project.RootTask.Children.GetById(1);

        // Atur formula untuk atribut yang diperluas
        var extendedAttributeDefinition1 = project.ExtendedAttributes[0];
        extendedAttributeDefinition1.Alias = "Days from finish to deadline";
        extendedAttributeDefinition1.Formula = "[Deadline] - [Finish]";

        // Atur Batas Waktu Tugas dan simpan proyek
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

// Metode bantuan untuk membuat proyek
public static Project CreateTestProjectWithCustomField7()
{
    var project = new Project(DataDir + "Blank2010.mpp");
    project.Set(Prj.StartDate, new DateTime(2015, 3, 6, 8, 0, 0));

    // Tambahkan tugas baru dengan atribut tambahan
    var task = project.RootTask.Children.Add("Task");
    var extendedAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text5, "My Ext Attr");
    project.ExtendedAttributes.Add(extendedAttributeDefinition);
    var extendedAttribute = extendedAttributeDefinition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(extendedAttribute);

    // Tambahkan sumber daya dan penugasan sumber daya
    var rsc = project.Resources.Add("Rsc");
    project.ResourceAssignments.Add(task, rsc);
    return project;
}
```

Menampilkan cara menggunakan fungsi matematika umum dengan atribut ekstensi.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Atur Rumus
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Cetak nilai atribut ekstensi
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
        // Atur Rumus
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Cetak nilai atribut ekstensi
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Atur Rumus
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Cetak nilai atribut ekstensi
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

### Lihat Juga

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


