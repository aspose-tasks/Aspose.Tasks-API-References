---
title: "ExtendedAttributeDefinitionCollection.Insert"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinitionCollection method. निर्दिष्ट इंडेक्स पर निर्दिष्ट आइटम डालता है"
type: docs
weight: 120
url: /hi/net/aspose.tasks/extendedattributedefinitioncollection/insert/
---
## ExtendedAttributeDefinitionCollection.Insert method

निर्दिष्ट सूचकांक पर निर्दिष्ट आइटम डालता है।

```csharp
public void Insert(int index, ExtendedAttributeDefinition item)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| इंडेक्स | Int32 | वह निर्दिष्ट शून्य-आधारित इंडेक्स जहाँ आइटम को सम्मिलित किया जाना चाहिए। |
| आइटम | ExtendedAttributeDefinition | इस संग्रह में सम्मिलित करने के लिए निर्दिष्ट आइटम। |

## उदाहरण

विस्तारित एट्रिब्यूट डिफिनिशन संग्रहों का उपयोग कैसे करें, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

if (!project.ExtendedAttributes.IsReadOnly)
{
    if (project.ExtendedAttributes.Count > 0)
    {
        // विस्तारित एट्रिब्यूट डिफिनिशन साफ़ करें
        project.ExtendedAttributes.Clear();
    }
}

// एक टास्क के लिए विस्तारित एट्रिब्यूट परिभाषा बनाएं
var taskDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(taskDefinition);

Console.WriteLine("Iterate over extended attributes of " + project.ExtendedAttributes.ParentProject.Get(Prj.Name) + " project: ");
foreach (var attribute in project.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

Console.WriteLine();

// विस्तारित एट्रिब्यूट डिफिनिशन के साथ काम करें...
var resourceDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My cost");

if (!project.ExtendedAttributes.Contains(resourceDefinition))
{
    project.ExtendedAttributes.Add(resourceDefinition);
}

// विस्तारित एट्रिब्यूट डिफिनिशन के साथ काम करें...
var resourceDefinition2 = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Number, ExtendedAttributeResource.Cost1, "My Cost 2");

if (project.ExtendedAttributes.IndexOf(resourceDefinition2) < 0)
{
    project.ExtendedAttributes.Insert(0, resourceDefinition2);
}

// विस्तारित एट्रिब्यूट डिफिनिशन के साथ काम करें...

// इंडेक्स द्वारा विस्तारित एट्रिब्यूट हटाएँ
project.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Print project's extended attributes: ");
Console.WriteLine("Count of project's extended attribute definitions: " + project.ExtendedAttributes.Count);

// संग्रह इंडेक्स एक्सेस का उपयोग करें
Console.WriteLine("Attribute 1 Alias: " + project.ExtendedAttributes[0].Alias);
Console.WriteLine("Attribute 1 CfType: " + project.ExtendedAttributes[0].CfType);
Console.WriteLine("Attribute 2 Alias: " + project.ExtendedAttributes[1].Alias);
Console.WriteLine("Attribute 2 CfType: " + project.ExtendedAttributes[1].CfType);

var otherProject = new Project();

// एट्रिब्यूट्स को अन्य प्रोजेक्ट में कॉपी करें
var attributes = new ExtendedAttributeDefinition[project.ExtendedAttributes.Count];
project.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherProject.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other project's extended attributes: ");
foreach (var attribute in otherProject.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

// सभी विस्तारित एट्रिब्यूट परिभाषाएँ हटाएँ
List<ExtendedAttributeDefinition> definitions = project.ExtendedAttributes.ToList();
foreach (var definition in definitions)
{
    project.ExtendedAttributes.Remove(definition);
}
```

### संबंधित देखें

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttributeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../extendedattributedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


