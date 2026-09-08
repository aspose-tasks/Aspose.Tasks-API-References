---
title: "SaveTemplateOptions.RemoveFixedCosts"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveTemplateOptions 속성. 프로젝트 템플릿의 모든 고정 비용을 제거할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks.saving/savetemplateoptions/removefixedcosts/
---
## SaveTemplateOptions.RemoveFixedCosts property

프로젝트 템플릿의 모든 고정 비용을 제거할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool RemoveFixedCosts { get; set; }
```

## 예제

옵션을 사용하여 프로젝트를 템플릿으로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// 템플릿 저장 옵션을 생성합니다
// 그리고 해당 속성을 조정합니다
var options = new SaveTemplateOptions
{
    // 프로젝트 템플릿의 모든 고정 비용을 제거할지 여부를 나타내는 값을 설정합니다
    RemoveFixedCosts = true,

    // 프로젝트 템플릿의 모든 실제 값을 제거할지 여부를 나타내는 값을 설정합니다
    RemoveActualValues = true,

    // 프로젝트 템플릿의 리소스 요금을 제거할지 여부를 나타내는 값을 설정합니다
    RemoveResourceRates = true,

    // 프로젝트 템플릿의 모든 기준값을 제거할지 여부를 나타내는 값을 설정합니다
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### 또 보기

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


