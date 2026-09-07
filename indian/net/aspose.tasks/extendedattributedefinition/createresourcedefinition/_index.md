---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition मेथड। एक फ़ैक्टरी मेथड जो एक सरल विस्तारित विशेषता परिभाषा बनाता है जिसे Microsoft Project में None के रूप में दिखाया जाता है। इसका CalculationType None के बराबर है और इसे केवल Resource में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको customFieldType, fieldId और alias निर्दिष्ट करने की आवश्यकता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

फ़ैक्टरी मेथड जो एक सरल विस्तारित विशेषता परिभाषा बनाता है, जिसे Microsoft Project में "None" के रूप में दिखाया जाता है। इसका [`CalculationType`](../calculationtype/) None के बराबर है और इसे केवल Resource में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको *customFieldType*, *fieldId* और *alias* निर्दिष्ट करने की आवश्यकता है।

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| customFieldType | CustomFieldType | निर्दिष्ट [`CustomFieldType`](../../customfieldtype/) प्रकार। |
| fieldId | ExtendedAttributeResource | निर्दिष्ट [`ExtendedAttributeResource`](../../extendedattributeresource/) फ़ील्ड ID। |
| उपनाम | स्ट्रिंग | निर्दिष्ट स्ट्रिंग उपनाम। |

### रिटर्न वैल्यू

निर्दिष्ट *customFieldType*, *fieldId* और *alias* के साथ [`ExtendedAttributeDefinition`](../) क्लास का इंस्टेंस बनाया गया।

## उदाहरण

इस उदाहरण का उपयोग करके एक कस्टम टेक्स्ट फ़ील्ड परिभाषा बनाएं:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

दिखाता है कि कैसे विस्तारित विशेषता को एक रिसोर्स असाइनमेंट में जोड़ा जाए।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// नया टास्क और रिसोर्स जोड़ें
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // "Resource Usage" दृश्य में दिखाई देने वाले कस्टम एट्रिब्यूट्स को ExtendedAttributeDefinition.CreateResourceDefinition मेथड से बनाया जा सकता है।
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // एट्रिब्यूट का प्रकार "Cost" है, इसलिए हमें "NumericValue" प्रॉपर्टी का उपयोग करना होगा।
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // "Task Usage" दृश्य में दिखाई देने वाले कस्टम एट्रिब्यूट्स को ExtendedAttributeDefinition.CreateTaskDefinition मेथड से बनाया जा सकता है।
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // एट्रिब्यूट का प्रकार "Cost" है, इसलिए हमें "NumericValue" प्रॉपर्टी का उपयोग करना होगा।
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

फ़ैक्टरी मेथड जो एक सरल विस्तारित विशेषता परिभाषा बनाता है, जिसे Microsoft Project में "None" के रूप में दिखाया जाता है। इसका [`CalculationType`](../calculationtype/) None के बराबर है और इसे केवल Resource में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको *fieldId* और *alias* निर्दिष्ट करने की आवश्यकता है। फ़ील्ड प्रकार field id से अनुमानित किया जाता है।

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | निर्दिष्ट [`ExtendedAttributeResource`](../../extendedattributeresource/) फ़ील्ड ID। |
| उपनाम | स्ट्रिंग | निर्दिष्ट स्ट्रिंग उपनाम। |

### रिटर्न वैल्यू

निर्दिष्ट *fieldId* और *alias* के साथ [`ExtendedAttributeDefinition`](../) क्लास का इंस्टेंस बनाया गया।

## उदाहरण

इस उदाहरण का उपयोग करके एक कस्टम टेक्स्ट फ़ील्ड परिभाषा बनाएं:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

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

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


