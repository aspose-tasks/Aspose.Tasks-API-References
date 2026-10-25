---
title: "Asn.LevelingDelay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Penundaan yang disebabkan oleh penyeimbangan"
type: docs
weight: 310
url: /id/net/aspose.tasks/asn/levelingdelay/
---
## Asn.LevelingDelay field

Keterlambatan yang disebabkan oleh leveling.

```csharp
public static readonly Key<Duration, AsnKey> LevelingDelay;
```

## Contoh

Menampilkan cara membaca/menulis properti Asn.Delay dan Asn.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Delay, project.GetDuration(0, TimeUnitType.Day));

Console.WriteLine("Delay: " + assignment.Get(Asn.Delay));
Console.WriteLine("Leveling Delay: " + assignment.Get(Asn.LevelingDelay));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


