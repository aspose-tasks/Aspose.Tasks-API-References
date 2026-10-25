---
title: "OutlineCodeDefinition.Values"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineCodeDefinition özelliği. OutlineValueCollection nesnesini alır. Bu ana hat kodu ile ilişkili tablonun değerleri"
type: docs
weight: 150
url: /tr/net/aspose.tasks/outlinecodedefinition/values/
---
## OutlineCodeDefinition.Values property

OutlineValueCollection nesnesini alır. Bu ana hat koduyla ilişkili tablonun değerleri.

```csharp
public OutlineValueCollection Values { get; }
```

## Örnekler

Yeni ana hat kodlarının nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "project.mpp");

// Ana hat kodunu ve onun ana hat maskesini tanımla
var code1 = new OutlineCodeDefinition();
code1.Alias = "New task outline code1";
code1.FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString();
code1.FieldName = "Outline Code1";
var mask = new OutlineMask();
mask.Separator = "+";
mask.Level = 1;
mask.Type = MaskType.Numbers;
code1.Masks.Add(mask);

// Ana hat değeri ekle
var value = new OutlineValue();
value.Description = "Value description";
value.ValueId = 1;
value.Value = "123456";
value.Type = OutlineValueType.Number;
code1.Values.Add(value);

// Ana hat kodunu projeye ekle
project.OutlineCodes.Add(code1);

// Ana hat kodunu ve onun ana hat maskesini tanımla
var code2 = new OutlineCodeDefinition();
code2.Alias = "New rsc outline code2";
code2.FieldId = ((int)ExtendedAttributeResource.OutlineCode2).ToString();
code2.FieldName = "Outline Code2";
var mask2 = new OutlineMask();
mask2.Separator = "/";
mask2.Level = 1;
mask2.Type = MaskType.Numbers;
code2.Masks.Add(mask2);

// Ana hat değeri ekle
var value2 = new OutlineValue();
value2.Description = "Value2 description";
value2.ValueId = 2;
value2.Value = "987654";
value2.Type = OutlineValueType.Number;
code2.Values.Add(value2);

// Ana hat kodunu projeye ekle
project.OutlineCodes.Add(code2);

project.Save(OutDir + "Updated_project_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [OutlineValueCollection](../../outlinevaluecollection/)
* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


