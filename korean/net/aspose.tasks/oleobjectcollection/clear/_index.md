---
title: "OleObjectCollection.Clear"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OleObjectCollection 메서드. 컬렉션을 비웁니다. 이러한 변경 사항을 지속하려면 new MPPSaveOptions WriteViewData true와 함께 project.Save를 호출해야 합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

컬렉션을 비웁니다. 이러한 변경 사항을 지속하려면 new MPPSaveOptions { WriteViewData = true; }와 함께 project.Save를 호출해야 합니다.

```csharp
public void Clear()
```

## 예제

OLE 객체를 비우고 이러한 변경 사항을 지속하는 방법.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

지정된 프로젝트에서 OLE 객체를 제거하는 방법을 보여줍니다.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### 또 보기

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


