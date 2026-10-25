---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskLink property. LagFormat के आधार पर लैग अवधि को प्राप्त करता है या सेट करता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

LagFormat के आधार पर लेग अवधि को प्राप्त करता है या सेट करता है।

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | जब LagFormat TimeUnitType.Percent होने पर TaskLinks के लिए मान सेट करने का प्रयास किया जाता है। |

## टिप्पणियाँ

लिंक लैग प्रतिशत मान हो सकता है (LagFormat TimeUnitType.Percent है)। इस मामले में अवधि को PredTask की अवधि के प्रतिशत के रूप में गणना किया जाता है। अन्यथा मेथड TimeSpan मान लौटाता है जो TaskLink के लैग को दर्शाता है।

### संबंधित देखें

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


