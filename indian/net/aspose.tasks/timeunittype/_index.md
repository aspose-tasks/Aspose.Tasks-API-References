---
title: "Enum TimeUnitType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TimeUnitType enum. समय इकाई के प्रकार को निर्दिष्ट करता है"
type: docs
weight: 2570
url: /hi/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

समय इकाई के प्रकार को निर्दिष्ट करता है।

```csharp
public enum TimeUnitType : sbyte
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | अपरिभाषित मान दर्शाता है कि फ़ील्ड मूल प्रोजेक्ट फ़ाइल में परिभाषित नहीं था। |
| Minute | `0` | मिनट समय इकाई प्रकार दर्शाता है। |
| ElapsedMinute | `1` | बीता हुआ मिनट समय इकाई प्रकार दर्शाता है। |
| Hour | `2` | घंटा समय इकाई प्रकार दर्शाता है। |
| ElapsedHour | `3` | बीता हुआ घंटा समय इकाई प्रकार दर्शाता है। |
| Day | `4` | दिन समय इकाई प्रकार दर्शाता है। |
| ElapsedDay | `5` | बीता हुआ दिन समय इकाई प्रकार दर्शाता है। |
| Week | `6` | सप्ताह समय इकाई प्रकार दर्शाता है। |
| ElapsedWeek | `7` | बीता हुआ सप्ताह समय इकाई प्रकार दर्शाता है। |
| Month | `8` | महीना समय इकाई प्रकार दर्शाता है। |
| ElapsedMonth | `9` | बीता हुआ महीना समय इकाई प्रकार दर्शाता है। |
| Percent | `10` | प्रतिशत समय इकाई प्रकार दर्शाता है। |
| ElapsedPercent | `11` | बीता हुआ प्रतिशत समय इकाई प्रकार दर्शाता है। |
| Null | `12` | नल समय इकाई प्रकार दर्शाता है। |
| MinuteEstimated | `13` | मिनट अनुमानित समय इकाई प्रकार दर्शाता है। |
| ElapsedMinuteEstimated | `14` | बीता हुआ मिनट अनुमानित समय इकाई प्रकार दर्शाता है। |
| HourEstimated | `15` | घंटा अनुमानित समय इकाई प्रकार दर्शाता है। |
| ElapsedHourEstimated | `16` | बीता हुआ घंटा अनुमानित समय इकाई प्रकार दर्शाता है। |
| DayEstimated | `17` | दिन अनुमानित समय इकाई प्रकार दर्शाता है। |
| ElapsedDayEstimated | `18` | बीता हुआ दिन अनुमानित समय इकाई प्रकार दर्शाता है। |
| WeekEstimated | `19` | सप्ताह अनुमानित समय इकाई प्रकार दर्शाता है। |
| ElapsedWeekEstimated | `20` | बीता हुआ सप्ताह अनुमानित समय इकाई प्रकार दर्शाता है। |
| MonthEstimated | `21` | महीना अनुमानित समय इकाई प्रकार दर्शाता है। |
| ElapsedMonthEstimated | `22` | बीता हुआ महीना अनुमानित समय इकाई प्रकार दर्शाता है। |
| PercentEstimated | `23` | प्रतिशत अनुमानित समय इकाई प्रकार दर्शाता है। |
| ElapsedPercentEstimated | `24` | समय इकाई प्रकार के अनुमानित बीते प्रतिशत को दर्शाता है। |
| Year | `25` | वर्ष समय इकाई प्रकार को दर्शाता है। |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

दिखाता है कि अवधि को विभिन्न समय इकाई प्रकारों में कैसे बदलें।

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// एक कार्य प्राप्त करें ताकि उसकी अवधि को विभिन्न स्वरूपों में गणना किया जा सके
var task = project.RootTask.Children.GetById(1);

// मिनट, दिन, घंटे, सप्ताह और महीने में अवधि प्राप्त करें
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


