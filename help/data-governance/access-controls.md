---
title: Controles de acceso
description: Obtenga información sobre cómo configurar los controles de acceso en Marketing Campaign Analytics.
feature: Administration
exl-id: c9ec97d9-b9a2-41f5-8626-1cf967d5d7fe
autotag-review: '2026-05-01T09:20:37.287Z'
TQID: 'https://experienceleague.adobe.com/ThO2ylnzexAPA1qczBJ5EEfHErHphVQ3XjXug71w6A0'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Marketing Campaign Analytics
feature_v2:
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized data
  - id: e0abf868-dae2-4c1c-83e9-b21799232845
    internal-label: Datasets
  - id: fe2edbb1-46f9-4347-a27c-577cab3640cb
    internal-label: Administration
subfeature_v2:
  - id: abe9e290-7d2f-4131-b71e-ef9900865044
    internal-label: Access control
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 9d6bd798e97d36d49b7753dc9574b102efb3d6bf
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 3%
---
# Controles de acceso

{{mm-mca-rebranding}}

El control de acceso para Marketing Campaign Analytics se proporciona a través de Experience Platform en [Adobe Admin Console](https://adminconsole.adobe.com/) y de [Permisos](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#platform-permissions) en Experience Platform. Esta funcionalidad aprovecha los perfiles de producto en Admin Console, que vinculan a los usuarios con permisos y entornos limitados.

Para obtener más información sobre el control de acceso, vea [Información general sobre el control de acceso](https://experienceleague.adobe.com/es/docs/experience-platform/access-control/home).

## Control de acceso basado en roles

Consulte [Administración](../main-guide/administration.md) sobre cómo configurar permisos de acceso basados en roles para usuarios y grupos de usuarios de Marketing Campaign Analytics en Experience Platform.

## Control de acceso basado en atributos

[El control de acceso basado en atributos](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview) es una funcionalidad de Experience Platform que permite a los administradores controlar el acceso a objetos específicos o a funcionalidades basadas en atributos. Los atributos pueden ser metadatos añadidos a un objeto, como una etiqueta añadida a un campo o segmento de esquema. Un administrador define directivas de acceso que incluyen atributos para administrar permisos de acceso de usuarios.

Esta funcionalidad le permite etiquetar campos de esquema del Modelo de datos de experiencia (XDM) con etiquetas que definen ámbitos organizativos o de uso de datos. En paralelo, los administradores pueden utilizar la interfaz de administración de usuarios y funciones para definir directivas de acceso en los campos de esquema XDM. Y administrar mejor el acceso dado a usuarios o grupos de usuarios (usuarios internos, externos o de terceros). Además, el control de acceso basado en atributos permite a los administradores gestionar el acceso a segmentos específicos.

Mediante el control de acceso basado en atributos, los administradores pueden controlar el acceso de los usuarios a los datos personales confidenciales (SPD) y a la información de identificación personal (PII) en todos los flujos de trabajo y recursos de la plataforma. Los administradores pueden definir funciones de usuario que solo tengan acceso a campos y datos específicos que correspondan a esos campos.

Al configurar reglas de conjuntos de datos para conjuntos de datos armonizados, el control de acceso [basado en atributos](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview) de Experience Platform se aplica en el nivel de campo. Un campo está restringido cuando se adjunta una etiqueta a un campo de esquema. Y se habilita una directiva activa que deniega el acceso al campo. Como resultado:

* no ve los campos de esquema que están restringidos al crear una regla de conjunto de datos,
* no puede ver ni editar la asignación de uno o varios campos de esquema que están restringidos. Cuando edita o ve una regla del conjunto de datos que contiene estos campos restringidos, verá la siguiente pantalla.
  ![Acción no permitida](/help/assets/action-not-permitted.png)
