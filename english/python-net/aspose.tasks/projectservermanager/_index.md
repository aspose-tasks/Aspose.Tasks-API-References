---
title: ProjectServerManager
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 870
url: /python-net/aspose.tasks/projectservermanager/
---

## ProjectServerManager class

The class which provides the methods to read and to perform operations on projects in the specified Project Online account or<br/>            in the specified on-premise Project Server instance (Project Server's versions 2016 and 2019 are supported).

The ProjectServerManager type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|ProjectServerManager(credentials)|Initializes a new instance of the [ProjectServerManager](/tasks/python-net/aspose.tasks/projectservermanager/) class.|
## Methods
| Name | Description |
| :- | :- |
|update_project(project)|Updates existing project in Project Server\Project Online instance using default save options. The existing project will be overwritten.|
|update_project(project, save_options)|Updates existing project in Project Server\Project Online instance using the specified save options. The existing project will be overwritten.|
|create_new_project(project)|Creates new project in Project Server\Project Online instance using default save options.|
|create_new_project(project, save_options)|Creates new project in Project Server\Project Online instance using the specified save options.|
|get_project(project_guid)|Gets the project with the specified guid from the Project Online account \ Project Server instance.|
|get_project_raw_data(project_guid)|Gets the project's binary data for troubleshooting purposes.|
|get_project_list()|Gets the list of projects from 'Working' store of the current Project Online account \ Project Server instance.|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

