---
title: "RiskPattern"
second_title: "Aspose.Tasks för Python via .NET API-referens"
description: 
type: docs
weight: 60
url: /sv/python-net/aspose.tasks.riskanalysis/riskpattern/
---

## RiskPattern class

Representerar ett riskmönster för en projektuppgift.

Typen RiskPattern visar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| RiskPattern(task) | Initierar en ny instans av klassen [RiskPattern](/tasks/python-net/aspose.tasks.riskanalysis/riskpattern/). |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| task | Hämtar en projektuppgift som detta riskmönster tillämpas på. |
| distribution | Hämtar eller anger sannolikhetsfördelningen som används i Monte Carlo-simulering.<br/>            Standardvärdet är ProbabilityDistributionType.Normal. |
| confidence_level | Hämtar eller anger konfidensnivån som motsvarar den procentandel av tiden som de faktiska genererade värdena kommer att ligga inom optimistiska och pessimistiska uppskattningar.<br/>            Standardvärdet är CL99. |
| optimistic | Hämtar eller anger den procentandel av den mest sannolika uppgiftens varaktighet som kan inträffa i det bästa möjliga projektscenariot.<br/>            Standardvärdet är 75, vilket betyder att om den uppskattade specificerade uppgiftens varaktighet är 4 dagar så blir den optimistiska varaktigheten 3 dagar. |
| pessimistic | Hämtar eller anger den procentandel av den mest sannolika uppgiftens varaktighet som kan inträffa i det värsta möjliga projektscenariot.<br/>            Standardvärdet är 125, vilket betyder att om den uppskattade specificerade uppgiftens varaktighet är 4 dagar så blir den pessimistiska varaktigheten 5 dagar. |

### Se även

* namespace [aspose.tasks.riskanalysis](/tasks/python-net/aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](/tasks/python-net/)

