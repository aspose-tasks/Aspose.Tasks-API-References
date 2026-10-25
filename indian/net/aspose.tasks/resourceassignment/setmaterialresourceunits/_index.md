---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment मेथड। एक भौतिक संसाधन के असाइनमेंट के लिए इकाइयों को सेट करता है जिसमें परिवर्तनीय सामग्री खपत होती है। परिवर्तनीय सामग्री खपत का अर्थ है कि जैसे ही असाइनमेंट की अवधि बदलती है, उपयोग की गई सामग्री की मात्रा अनुपातिक रूप से बदलती है।"
type: docs
weight: 760
url: /hi/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

परिवर्तनीय सामग्री खपत वाले सामग्री संसाधन के असाइनमेंट के लिए इकाइयाँ सेट करता है। परिवर्तनीय सामग्री खपत का अर्थ है कि असाइनमेंट अवधि बदलने पर उपयोग की गई सामग्री की मात्रा समानुपातिक रूप से बदलती है।

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| इकाइयाँ | Double | समय अवधि में संचित इकाइयों की संख्या। |
| rateScaleType | RateScaleType | समय अवधि जिसमें इकाई मूल्य संचित होता है। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | यदि मेथड को गैर-भौतिक संसाधन के असाइनमेंट के लिए बुलाया जाता है। |

## टिप्पणियाँ

उदाहरण के लिए, '123/month' सेट करने के लिए, SetUnitsScaled(123D, RateScaleType.Month) को कॉल किया जाना चाहिए।

## उदाहरण

एक सामग्री संसाधन के असाइनमेंट के लिए परिवर्ती सामग्री खपत (जैसे '10/day' या '1/week') सेट करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// मान लीजिए हम '1/week' सामग्री खपत सेट करना चाहते हैं।
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

### संबंधित देखें

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


