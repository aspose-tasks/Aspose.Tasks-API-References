---
title: "MPPSaveOptions.WriteFilters"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MPPSaveOptions प्रॉपर्टी। यह मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय फ़िल्टर डेटा लिखा जाए या नहीं। फ़िल्टर डेटा में Project.TaskFilters और Project.ResourceFilters संग्रह शामिल हैं।"
type: docs
weight: 50
url: /hi/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय फ़िल्टर डेटा लिखने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। फ़िल्टर डेटा में Project.TaskFilters और Project.ResourceFilters संग्रह शामिल हैं।

```csharp
public bool WriteFilters { get; set; }
```

## टिप्पणियाँ

वर्तमान में MSP 2010 या नए फ़ॉर्मेट्स के लिए समर्थित है।

## उदाहरण

दिखाता है कि MPP प्रोजेक्ट में नया टास्क फ़िल्टर कैसे जोड़ें और सहेजें।

```csharp
Project project = new Project();

project.TaskFilters.Clear();
project.ResourceFilters.Clear();

var filter = new Filter();
filter.Name = "New Task Filter";
filter.FilterType = ItemType.TaskItem;
filter.ShowInMenu = true;
filter.ShowRelatedSummaryRows = true;

filter.Criteria = new FilterCriteria();

var criteria1 = new FilterCriteria();
criteria1.Field = Field.TaskNumber13;
criteria1.Test = FilterComparisonType.IsLessThan;
criteria1.Values[0] = 34.3D;

filter.Criteria.CriteriaRows.Add(criteria1);
project.TaskFilters.Add(filter);

SimpleSaveOptions options = new MPPSaveOptions() { WriteFilters = true };
project.Save(OutDir + "output_new_filter.mpp", options);
```

### संबंधित देखें

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


