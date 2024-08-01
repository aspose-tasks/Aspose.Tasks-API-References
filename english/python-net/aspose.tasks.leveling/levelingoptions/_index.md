---
title: LevelingOptions
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.tasks.leveling/levelingoptions/
---

## LevelingOptions class

Allows to specify parameters of resource leveling.

The LevelingOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|LevelingOptions()|Initializes a new instance of the [LevelingOptions](/tasks/python-net/aspose.tasks.leveling/levelingoptions/) class.|
## Properties
| Name | Description |
| :- | :- |
|start_date|Gets or sets leveling period start date. The default value is the project`s start date.|
|finish_date|Gets or sets leveling period end date. The default value is the project`s finish date.|
|resources|Gets or sets the list of the resources which will be leveled. If null is set, all project resources will be leveled.|
|leveling_order|Gets the order in which the leveling algorithm delays tasks that have overallocations.<br/>            After determination of tasks causing the overallocation and which tasks can be delayed, the specified order is used which task should be delayed first.|
|message_level|Gets or sets level of log messages emitted by Aspose.Tasks during resource leveling.|
|message_handler|Gets or sets message handler callback which can be used to intercept log messages produced by Aspose.Tasks during resource leveling.|

### See Also

* namespace [aspose.tasks.leveling](/tasks/python-net/aspose.tasks.leveling/)
* assembly [Aspose.Tasks](/tasks/python-net/)

