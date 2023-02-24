---
title: ViewSettings
second_title: .NET API 참조용 Aspose.Tasks
description: 보기를 가져오거나 설정합니다Viewaspose.tasks.saving/saveoptions/view/  렌더링합니다. 이 옵션을 사용하여 PDF HTML 또는 이미지 형식으로 저장할 보기를 명시적으로 지정할 수 있습니다. 이 속성이 설정되면PresentationFormataspose.tasks.visualization/presentationformat/ 프로젝트 저장 시 속성은 무시됩니다. 보기는 다음 화면 중 하나여야 합니다Screenaspose.tasks/view/screen/  Gantt TaskSheet TaskUsage ResourceSheet ResourceUsage
type: docs
weight: 240
url: /ko/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

보기를 가져오거나 설정합니다([`View`](../view/) ) 렌더링합니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장할 보기를 명시적으로 지정할 수 있습니다. 이 속성이 설정되면[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) 프로젝트 저장 시 속성은 무시됩니다. 보기는 다음 화면 중 하나여야 합니다(([`Screen`](../../../aspose.tasks/view/screen/) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

```csharp
public View ViewSettings { get; set; }
```

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | set 메소드 호출 시 Screen 속성값이 지원하지 않는 View 클래스의 인스턴스가 제공됩니다. |

### 또한보십시오

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* 네임스페이스 [Aspose.Tasks.Saving](../../saveoptions/)
* 집회 [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->