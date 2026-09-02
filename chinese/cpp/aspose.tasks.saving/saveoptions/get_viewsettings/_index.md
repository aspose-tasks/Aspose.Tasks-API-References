---
title: "Aspose::Tasks::Saving::SaveOptions::get_ViewSettings 方法"
linktitle: "get_ViewSettings"
articleTitle: "get_ViewSettings"
second_title: "Aspose.Tasks for C++"
description: "获取一个视图 ( View ) 用于渲染。"
type: docs
weight: 240
url: /zh/cpp/aspose.tasks.saving/saveoptions/get_viewsettings/
---

## get_ViewSettings {#get_viewsettings}

获取要渲染的视图（ View ）。您可以使用此选项显式指定应保存为 PDF、HTML 或 Image 格式的视图。如果设置了此属性，保存项目时会忽略 Visualization::PresentationFormat 属性。View 应来自以下屏幕之一 (( Aspose::Tasks::View::Screen ))：（Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage）

**Returns:** System::SharedPtr< Aspose::Tasks::View > Aspose::Tasks::Saving::

```cpp
get_ViewSettings()
```

