---
title: "Enum Month"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Month enum। महीने को निर्दिष्ट करता है।"
type: docs
weight: 1040
url: /hi/net/aspose.tasks/month/
---
## Month enumeration

माह को निर्दिष्ट करता है।

```csharp
public enum Month
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | मूल प्रोजेक्ट फ़ाइल में मान परिभाषित नहीं था, यह दर्शाता है। |
| January | `0` | जनवरी महीने को दर्शाता है। |
| February | `1` | फ़रवरी महीने को दर्शाता है। |
| March | `2` | मार्च महीने को दर्शाता है। |
| April | `3` | अप्रैल महीने को दर्शाता है। |
| May | `4` | मई महीने को दर्शाता है। |
| June | `5` | जून महीने को दर्शाता है। |
| July | `6` | जुलाई महीने को दर्शाता है। |
| August | `7` | अगस्त महीने को दर्शाता है। |
| September | `8` | सितंबर महीने को दर्शाता है। |
| October | `9` | अक्टूबर महीने को दर्शाता है। |
| November | `10` | नवंबर महीने को दर्शाता है। |
| December | `11` | दिसंबर महीने को दर्शाता है। |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

नए पुनरावर्ती कार्य बनाते समय वर्ष-दिन दोहराव के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


