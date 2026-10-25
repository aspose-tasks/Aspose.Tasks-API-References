---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition मेथड। एक नया विस्तारित एट्रिब्यूट बनाता है जिसका फ़ील्ड ID इस ऑब्जेक्ट के फ़ील्ड ID मान के बराबर होता है"
type: docs
weight: 310
url: /hi/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

एक नया विस्तारित गुण बनाता है जिसमें फ़ील्ड आईडी इस ऑब्जेक्ट के फ़ील्ड आईडी मान के बराबर होता है।

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### रिटर्न वैल्यू

वापस बनायी गई इंस्टेंस [`ExtendedAttribute`](../../extendedattribute/) क्लास की, जिसका fieldID इस ऑब्जेक्ट के fieldID मान के बराबर है।

## उदाहरण

विस्तारित एट्रिब्यूट्स बनाने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// यदि कस्टम फ़ील्ड प्रोजेक्ट में मौजूद नहीं है, तो इसे बनाएं
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// परिभाषा से विस्तारित एट्रिब्यूट जेनरेट करें
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// टास्क में विस्तारित एट्रिब्यूट जोड़ें
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

एक नया विस्तारित गुण बनाता है जिसमें फ़ील्ड आईडी इस ऑब्जेक्ट के फ़ील्ड आईडी मान के बराबर होता है और निर्दिष्ट पाठ मान शामिल होता है।

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| textValue | स्ट्रिंग | निर्दिष्ट टेक्स्ट मान। |

### रिटर्न वैल्यू

वापस बनायी गई इंस्टेंस [`ExtendedAttribute`](../../extendedattribute/) क्लास की, जिसका fieldID इस ऑब्जेक्ट के fieldID मान के बराबर है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | यदि वर्तमान [`CfType`](../cftype/) 'Text' नहीं है |

## उदाहरण

विस्तारित एट्रिब्यूट परिभाषा बनाने और एट्रिब्यूट के स्ट्रिंग मान को सेट करने का तरीका दिखाता है जबकि यह निर्मित हो रहा है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// विस्तारित एट्रिब्यूट को 'Common Info' के बराबर मान के साथ बनाएं
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// विस्तारित एट्रिब्यूट को 'Common Info' मान से इनिशियलाइज़ करके जोड़ें
task.ExtendedAttributes.Add(extendedAttribute);
```

### संबंधित देखें

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

एक नया विस्तारित गुण बनाता है जिसमें फ़ील्ड आईडी इस ऑब्जेक्ट के फ़ील्ड आईडी मान के बराबर होता है और निर्दिष्ट संख्यात्मक मान शामिल होता है।

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| numericValue | Decimal | निर्दिष्ट संख्यात्मक मान। |

### रिटर्न वैल्यू

वापस बनायी गई इंस्टेंस [`ExtendedAttribute`](../../extendedattribute/) क्लास की, जिसका fieldID इस ऑब्जेक्ट के fieldID मान के बराबर है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | यदि वर्तमान [`CfType`](../cftype/) 'Number' या 'Cost' नहीं है |

## उदाहरण

विस्तारित एट्रिब्यूट परिभाषा बनाने और एट्रिब्यूट के दशमलव मान को सेट करने का तरीका दिखाता है जबकि यह निर्मित हो रहा है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// विस्तारित एट्रिब्यूट को 999m के बराबर मान के साथ बनाएं 
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// विस्तारित एट्रिब्यूट को 999m मान से इनिशियलाइज़ करके जोड़ें
task.ExtendedAttributes.Add(extendedAttribute);
```

### संबंधित देखें

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

एक नया विस्तारित गुण बनाता है जिसमें फ़ील्ड आईडी इस ऑब्जेक्ट के फ़ील्ड आईडी मान के बराबर होता है और निर्दिष्ट तिथि मान शामिल होता है।

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dateTimeValue | DateTime | निर्दिष्ट तिथि समय मान। |

### रिटर्न वैल्यू

वापस बनायी गई इंस्टेंस [`ExtendedAttribute`](../../extendedattribute/) क्लास की, जिसका fieldID इस ऑब्जेक्ट के fieldID मान के बराबर है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | यदि वर्तमान [`CfType`](../cftype/) 'Date', 'Start' या 'Finish' नहीं है |

## उदाहरण

दिखाता है कि विस्तारित गुण परिभाषा कैसे बनाएं और निर्माण के दौरान गुण का datetime मान कैसे सेट करें।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// DateTime.Now के बराबर मान के साथ विस्तारित गुण बनाएं
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// विस्तारित गुण जोड़ें
task.ExtendedAttributes.Add(extendedAttribute);
```

### संबंधित देखें

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

एक नया विस्तारित गुण बनाता है जिसमें फ़ील्ड आईडी इस ऑब्जेक्ट के फ़ील्ड आईडी मान के बराबर होता है और निर्दिष्ट अवधि मान शामिल होता है।

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| durationValue | अवधि | निर्दिष्ट अवधि मान। |

### रिटर्न वैल्यू

वापस बनायी गई इंस्टेंस [`ExtendedAttribute`](../../extendedattribute/) क्लास की, जिसका fieldID इस ऑब्जेक्ट के fieldID मान के बराबर है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | यदि वर्तमान [`CfType`](../cftype/) 'Duration' नहीं है |

## उदाहरण

दिखाता है कि विस्तारित गुण परिभाषा कैसे बनाएं और निर्माण के दौरान अवधि कैसे सेट करें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// विस्तारित गुण Duration1 = 2 दिन
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// कार्य में विस्तारित गुण जोड़ें
task.ExtendedAttributes.Add(extendedAttribute);
```

### संबंधित देखें

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

एक नया विस्तारित गुण बनाता है जिसमें फ़ील्ड आईडी इस ऑब्जेक्ट के फ़ील्ड आईडी मान के बराबर होता है और निर्दिष्ट फ़्लैग मान शामिल होता है।

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| flagValue | Boolean | निर्दिष्ट फ़्लैग मान। |

### रिटर्न वैल्यू

वापस बनायी गई इंस्टेंस [`ExtendedAttribute`](../../extendedattribute/) क्लास की, जिसका fieldID इस ऑब्जेक्ट के fieldID मान के बराबर है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | यदि वर्तमान [`CfType`](../cftype/) 'Flag' नहीं है |

## उदाहरण

दिखाता है कि विस्तारित एट्रिब्यूट परिभाषा कैसे बनाएं और निर्माण के दौरान फ़्लैग का मान कैसे सेट करें।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// बूलियन कस्टम फ़ील्ड के लिए परिभाषा बनाएं
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// एक एट्रिब्यूट बनाएं और प्रारंभिक मान को 'true' सेट करें
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### संबंधित देखें

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

निर्दिष्ट [`Value`](../../value/) आइटम से जुड़ा नया विस्तारित गुण बनाता है।

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| lookupValue | Value | निर्दिष्ट [`Value`](../../value/) आइटम। |

### रिटर्न वैल्यू

निर्दिष्ट [`Value`](../../value/) आइटम से जुड़ी बनाई गई [`ExtendedAttribute`](../../extendedattribute/) क्लास की इंस्टेंस लौटाता है।

## टिप्पणियाँ

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## उदाहरण

विशिष्ट मान का उपयोग करके नया [`ExtendedAttribute`](../../extendedattribute/) बनाने के लिए इस कोड का उपयोग करें:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

दिखाता है कि विस्तारित गुण परिभाषा कैसे बनाएं और निर्माण के दौरान मान कैसे सेट करें।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// ऊपर घोषित लुकअप टेबल के आधार पर एक कस्टम फ़ील्ड परिभाषा बनाएं।
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// किसी मान के लिए विस्तारित गुण बनाएं
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// कार्य में विस्तारित गुण जोड़ें
task.ExtendedAttributes.Add(extendedAttribute);
```

### संबंधित देखें

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


