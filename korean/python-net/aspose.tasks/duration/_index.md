---
title: "Duration"
second_title: "Aspose.Tasks for Python via .NET API 참조"
description: 
type: docs
weight: 260
url: /ko/python-net/aspose.tasks/duration/
---

## Duration class

프로젝트의 기간을 나타냅니다.

Duration 유형은 다음 멤버를 노출합니다:
## 생성자
| 이름 | 설명 |
| :- | :- |
| Duration() | Duration 클래스의 새 인스턴스를 초기화합니다 |
## 속성
| 이름 | 설명 |
| :- | :- |
| time_span | 이 Duration 객체의 [time_span](/tasks/python-net/aspose.tasks/duration/) 인스턴스를 가져옵니다. |
| time_unit | 이 객체의 시간 단위 유형을 가져옵니다. |
| is_estimated | 시간 단위가 추정되는지 여부를 나타내는 값을 가져옵니다. |
| is_elapsed | 시간 단위가 경과했는지 여부를 나타내는 값을 가져옵니다. |
## 메서드
| 이름 | 설명 |
| :- | :- |
| add(d) | 지정된 기간을 이 기간에 추가합니다. |
| add(val) | 지정된 double 값을 이 기간에 추가합니다. |
| subtract(d) | 지정된 기간을 이 기간 인스턴스에서 빼습니다. |
| subtract(val) | 지정된 double 값을 이 기간 인스턴스에서 빼습니다. |
| parse(p, value) | 지정된 문자열을 [Duration](/tasks/python-net/aspose.tasks/duration/) 구조체의 인스턴스로 변환합니다. |
| parse_time_span(value) | \"PT--H--M--S--\" 형식의 기간 문자열을 구문 분석합니다. |
| to_double() | Duration 객체를 float 값으로 변환합니다. |
| convert(time_unit_type) | Duration 객체를 지정된 시간 단위가 있는 다른 기간으로 변환합니다. |
| equals(other) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |

### 또 보기

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

