---
title: "ProjectServerManager"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 870
url: /fr/python-net/aspose.tasks/projectservermanager/
---

## ProjectServerManager class

La classe qui fournit les méthodes pour lire et effectuer des opérations sur les projets dans le compte Project Online spécifié ou<br/>            dans l'instance sur site de Project Server spécifiée (les versions 2016 et 2019 de Project Server sont prises en charge).

Le type ProjectServerManager expose les membres suivants :
## Constructeurs
| Nom | Description |
| :- | :- |
| ProjectServerManager(credentials) | Initialise une nouvelle instance de la classe [ProjectServerManager](/tasks/python-net/aspose.tasks/projectservermanager/). |
## Méthodes
| Nom | Description |
| :- | :- |
| update_project(project) | Met à jour le projet existant dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement par défaut. Le projet existant sera écrasé. |
| update_project(project, save_options) | Met à jour le projet existant dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement spécifiées. Le projet existant sera écrasé. |
| create_new_project(project) | Crée un nouveau projet dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement par défaut. |
| create_new_project(project, save_options) | Crée un nouveau projet dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement spécifiées. |
| get_project(project_guid) | Récupère le projet avec le guid spécifié depuis le compte Project Online \\ l'instance Project Server. |
| get_project_raw_data(project_guid) | Récupère les données binaires du projet à des fins de dépannage. |
| get_project_list() | Récupère la liste des projets depuis le magasin 'Working' du compte Project Online actuel \\ l'instance Project Server. |

### Voir aussi

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

