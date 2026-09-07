---
title: "क्लास DayTypeCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.DayTypeCollection क्लास। DayType ऑब्जेक्ट्स का संग्रह दर्शाता है"
type: docs
weight: 460
url: /hi/net/aspose.tasks/daytypecollection/
---
## DayTypeCollection class

[`DayType`](../daytype/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class DayTypeCollection : IList<DayType>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/daytypecollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/daytypecollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं; अन्यथा, false। |
| [Item](../../aspose.tasks/daytypecollection/item/) { get; set; } | निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/daytypecollection/add/)(DayType) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/daytypecollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/daytypecollection/contains/)(DayType) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/daytypecollection/copyto/)(DayType[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/daytypecollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [IndexOf](../../aspose.tasks/daytypecollection/indexof/)(DayType) | इस संग्रह में निर्दिष्ट आइटम का सूचकांक निर्धारित करता है। |
| [Insert](../../aspose.tasks/daytypecollection/insert/)(int, DayType) | निर्दिष्ट सूचकांक पर निर्दिष्ट आइटम डालता है। |
| [Remove](../../aspose.tasks/daytypecollection/remove/)(DayType) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [RemoveAt](../../aspose.tasks/daytypecollection/removeat/)(int) | निर्दिष्ट सूचकांक पर एक आइटम हटाता है। |

## उदाहरण

साप्ताहिक कैलेंडर अपवाद को परिभाषित करने के लिए सप्ताह के दिन के संग्रह का उपयोग कैसे करें दिखाता है।

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // \"Exception 2\" से दिन प्रकार को दिन प्रकार द्वारा हटाएँ
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// \"Exception 2\" से दिन प्रकार को अनुक्रमणिका द्वारा हटाएँ
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// अपवाद बदलें (प्रारंभिक प्रोजेक्ट डेटा में कोई अपवाद नहीं है)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// \"Exception 3\" के लिए सभी सप्ताह के दिन हटाएँ
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### संबंधित देखें

* enum [DayType](../daytype/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


