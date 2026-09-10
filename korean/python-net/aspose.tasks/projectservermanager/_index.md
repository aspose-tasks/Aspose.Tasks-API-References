---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Python via .NET API 참조"
description: 
type: docs
weight: 870
url: /ko/python-net/aspose.tasks/projectservermanager/
---

## ProjectServerManager class

지정된 Project Online 계정 또는<br/>            지정된 온프레미스 Project Server 인스턴스(지원되는 Project Server 버전은 2016 및 2019)에서 프로젝트를 읽고 작업을 수행하는 메서드를 제공하는 클래스입니다.

ProjectServerManager 유형은 다음 멤버를 노출합니다:
## 생성자
| 이름 | 설명 |
| :- | :- |
| ProjectServerManager(credentials) | [ProjectServerManager](/tasks/python-net/aspose.tasks/projectservermanager/) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드
| 이름 | 설명 |
| :- | :- |
| update_project(project) | 기본 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. 기존 프로젝트가 덮어쓰기됩니다. |
| update_project(project, save_options) | 지정된 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. 기존 프로젝트가 덮어쓰기됩니다. |
| create_new_project(project) | 기본 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스에 새 프로젝트를 생성합니다. |
| create_new_project(project, save_options) | 지정된 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스에 새 프로젝트를 생성합니다. |
| get_project(project_guid) | Project Online 계정 \\ Project Server 인스턴스에서 지정된 guid를 가진 프로젝트를 가져옵니다. |
| get_project_raw_data(project_guid) | 문제 해결을 위해 프로젝트의 바이너리 데이터를 가져옵니다. |
| get_project_list() | 현재 Project Online 계정 \\ Project Server 인스턴스의 'Working' 저장소에서 프로젝트 목록을 가져옵니다. |

### 또 보기

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

