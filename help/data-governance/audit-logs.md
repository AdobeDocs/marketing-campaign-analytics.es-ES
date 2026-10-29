---
title: Registros de auditoría
description: Obtenga información sobre cómo acceder a los registros de auditoría desde Marketing Campaign Analytics.
feature: Administration
exl-id: aa65aac5-bea4-43ff-b0d0-9e8a6a97d3ca
autotag-review: '2026-05-01T09:16:13.122Z'
TQID: 'https://experienceleague.adobe.com/ZH89ZDOEMDwbvU5QnPtpkDft0U121-JDrhgEBPDuV3Q'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Marketing Campaign Analytics
feature_v2:
  - id: f6633d1c-3d2d-4f48-95d4-4bbc9913db52
    internal-label: Data governance
  - id: fe2edbb1-46f9-4347-a27c-577cab3640cb
    internal-label: Administration
subfeature_v2:
  - id: bf7ac0fc-effb-4f0c-b93f-658412718d3c
    internal-label: Audits
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: 9d6bd798e97d36d49b7753dc9574b102efb3d6bf
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 6%
---
# Registros de auditoría

{{mm-mca-rebranding}}

Para aumentar la transparencia y la visibilidad de las actividades realizadas en el sistema, la actividad del usuario dentro del flujo de trabajo de Marketing Campaign Analytics se captura en los registros de auditoría de Experience Platform para comprender cualquier cambio impulsado por el usuario en las categorías de Marketing Campaign Analytics. Estos registros forman una pista de auditoría que puede ayudar con la resolución de problemas y pueden ayudar a su empresa a cumplir de forma eficaz con las políticas de administración de datos corporativos y los requisitos regulatorios.

<!-- 
DO WE HAVE TO ADD THIS
If you are subject to the Health Insurance Portability and Accountability Act (HIPAA) and create, receive, maintain, or transmit permitted sensitive personal data through Marketing Campaign Analytics, you are responsible for executing a BAA with Adobe and licensing Healthcare Shield.
-->

Un registro de auditoría informa de quién realizó qué acción y cuándo lo hizo. Cada acción registrada contiene metadatos que indican el tipo de acción, la fecha y la hora, el ID de correo electrónico del usuario que realizó la acción y los atributos adicionales relevantes de ese tipo de acción. Rastrea las acciones de creación, actualización y eliminación realizadas por los usuarios en Marketing Campaign Analytics.

Para inspeccionar el registro de auditoría, en la interfaz de Marketing Campaign Analytics:

1. Seleccione ![Lista de tareas](/help/assets/icons/TaskList.svg) **[!UICONTROL Audits]** de **[!UICONTROL PRIVACY]**.

1. En **[!UICONTROL Audits]**, puede encontrar **[!UICONTROL Activity log]**. El registro de actividad muestra las entradas de las siguientes categorías, acciones y estados de Marketing Campaign Analytics.

   | Categoría | Acción | Estado |
   |---|---|---|
   | Regla de conjunto de datos Marketing Campaign Analytics | Crear | Permitir o denegar |
   | Regla de conjunto de datos Marketing Campaign Analytics | Actualización | Permitir o denegar |
   | Regla de conjunto de datos Marketing Campaign Analytics | Eliminar | Permitir o denegar |
   | Campo de Marketing Campaign Analytics | Crear | Permitir o denegar |
   | Campo de Marketing Campaign Analytics | Actualización | Permitir o denegar |
   | Campo de Marketing Campaign Analytics | Eliminar | Permitir o denegar |
   | Marketing Campaign Analytics Marketing Touchpoint | Crear | Permitir o denegar |
   | Marketing Campaign Analytics Marketing Touchpoint | Actualización | Permitir o denegar |
   | Marketing Campaign Analytics Marketing Touchpoint | Eliminar | Permitir o denegar |
   | Conversión de Marketing Campaign Analytics | Crear | Permitir o denegar |
   | Conversión de Marketing Campaign Analytics | Actualización | Permitir o denegar |
   | Conversión de Marketing Campaign Analytics | Eliminar | Permitir o denegar |
   | Modelo Marketing Campaign Analytics | Crear | Permitir o denegar |
   | Modelo Marketing Campaign Analytics | Actualización | Permitir o denegar |
   | Modelo Marketing Campaign Analytics | Eliminar | Permitir o denegar |
   | Modelo Marketing Campaign Analytics | Rescore | Permitir o denegar |
   | Modelo Marketing Campaign Analytics | Clonar | Permitir o denegar |
   | Modelo Marketing Campaign Analytics | Tren/reciclaje | Permitir o denegar |
   | Modelo Marketing Campaign Analytics | Descargar o guardar metadatos | Permitir o denegar |
   | Plan de Marketing Campaign Analytics | Crear | Permitir o denegar |
   | Plan de Marketing Campaign Analytics | Actualización | Permitir o denegar |
   | Plan de Marketing Campaign Analytics | Cambiar modelo asociado | Permitir o denegar |
   | Armonización de datos de Marketing Campaign Analytics | Sincronización de déclencheur | Permitir o denegar |


1. Seleccione una entrada en el registro de actividad para abrir un panel y obtener más información.

   ![Auditoría de Marketing Campaign Analytics](/help/assets/mix-modeler-audit.png)

1. Para filtrar por el rango **[!UICONTROL Category]**, **[!UICONTROL Action]**, **[!UICONTROL Request ID]**, **[!UICONTROL User]**, **[!UICONTROL Status]** o **[!UICONTROL Date]**, seleccione ![Filtro](/help/assets/icons/Filter.svg).

1. Para modificar las columnas mostradas en el registro de actividad, seleccione ![Columnas](/help/assets/icons/ColumnSetting.svg) y, en el cuadro de diálogo **[!UICONTROL Customize table]**, seleccione las columnas que desea mostrar. Seleccione **[!UICONTROL Apply]** para aplicar la selección, **[!UICONTROL Cancel]** para cancelar la selección.

1. Para descargar el registro de auditoría, seleccione ![Descargar](/help/assets/icons/Download.svg) **[!UICONTROL Download log]**. En el cuadro de diálogo **[!UICONTROL Download log]**, seleccione **[!UICONTROL CSV]** o **[!UICONTROL JSON]** como formato y seleccione **[!UICONTROL Download]**.

## Acceso a los registros de auditoría

Cuando la función está habilitada para su organización, los registros de auditoría se recopilan automáticamente a medida que se produce la actividad. No es necesario habilitar manualmente la recopilación de registros de auditoría.

Para ver y exportar los registros de auditoría, se debe contar con el permiso de control Acceso a registros de auditoría. Para obtener información sobre cómo administrar los permisos individuales para las características de Marketing Campaign Analytics, consulte la [documentación de control de acceso](https://experienceleague.adobe.com/es/docs/experience-platform/access-control/home).
