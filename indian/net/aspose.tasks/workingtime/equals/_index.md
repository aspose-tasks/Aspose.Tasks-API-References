---
title: "WorkingTime.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WorkingTime मेथड। जाँच करता है कि वस्तुएँ समान हैं।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

जाँचता है कि वस्तुएँ समान हैं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | तुलना करने के लिए दूसरी वस्तु। |

### रिटर्न वैल्यू

यदि वस्तुएँ समान हों तो true, अन्यथा false।

## उदाहरण

दिखाता है कि कार्य समय समानता की जाँच कैसे करें।

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// कैलेंडरों की समानता को कार्य समय की from और to तिथियों के विरुद्ध जाँच किया जाता है।
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### संबंधित देखें

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


