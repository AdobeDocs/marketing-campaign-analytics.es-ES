---
title: Panel de datos armonizado
description: Aprenda a utilizar el tablero de información general de datos armonizado en Mix Modeler.
feature: Dashboard, Harmonized Data
exl-id: fbb01613-d648-4db1-a782-a7720b7a03ad
autotag-review: '2026-05-01T09:17:34.958Z'
TQID: 'https://experienceleague.adobe.com/umAqsiCgpFt4eLBuWPJahtwglXaQKD-iv91yCazIbkE'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Mix Modeler
feature_v2:
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized data
  - id: fe2edbb1-46f9-4347-a27c-577cab3640cb
    internal-label: Administration
subfeature_v2:
  - id: bc2f5225-03d4-4bc8-89ec-99d78c30e6dd
    internal-label: Conversions
  - id: b2d4aeb9-eabe-49f6-8edb-bb2862d5980b
    internal-label: Marketing touchpoints
  - id: c564971c-1597-4a46-a354-33d74ee8a5d1
    internal-label: Dashboard
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 6d83679f1c053f0be6eefd17929364d53221a31a
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%
---
# Datos armonizados

La ficha **[!UICONTROL Harmonized data]** de la página de inicio ![Mix Modeler](/help/assets/icons/Home.svg) **[!UICONTROL Overview]** proporciona información sobre los datos armonizados que ha configurado para que se utilicen como parte de los datos ingeridos y de la configuración de datos armonizados.

La descripción general muestra cuatro visualizaciones de la tarjeta de estado de KPI (fila superior) y otras seis visualizaciones configurables

Para cambiar el período de fecha de los datos que se mostrarán en las visualizaciones, escriba una fecha de inicio y una fecha de finalización manualmente o seleccione un período con ![Calendario](/help/assets/icons/Calendar.svg).

## Filtros de datos

Puede filtrar los datos mostrados para todas las visualizaciones mediante el panel ![Filtrar](/help/assets/icons/Filter.svg) **[!UICONTROL Category Filters]**.

Seleccione uno o más filtros para cada categoría (**[!UICONTROL Brands]**, **[!UICONTROL Campaigns]**, **[!UICONTROL Channels Type]**, **[!UICONTROL Conversion types]**, **[!UICONTROL Datasets]**, **[!UICONTROL Media types]**, **[!UICONTROL Source types]** y **[!UICONTROL Traffic Source]**).

Los filtros seleccionados se muestran sobre las visualizaciones en **[!UICONTROL FILTERING BY:]**.

1. Para quitar un filtro individual, seleccione ![Cerrar](/help/assets/icons/Close.svg) en el filtro, mostrado en **[!UICONTROL FILTERING BY:]**.

1. Puede borrar rápidamente todos los filtros usando **[!UICONTROL Clear All]**.

![Resumen de datos armonizados](/help/assets/harmonized-data-overview.png)


## Configuración de una visualización

Puede configurar cada visualización.

* En la visualización de la tarjeta de estado de KPI:

  1. Seleccione ![Editar](/help/assets/icons/Edit.svg) y ![Editar](/help/assets/icons/Edit.svg) **[!UICONTROL Edit data]** del menú contextual.

  1. En el diálogo **[!UICONTROL KPI status card]**:

     1. Seleccione un(a) **[!UICONTROL KPI]** de la lista.

     1. Seleccione **[!UICONTROL Apply]** para aplicar el cambio a la tarjeta. Seleccione **[!UICONTROL Cancel]** para cancelar el cambio.

* En las demás visualizaciones configurables:

  1. Seleccione ![Editar](/help/assets/icons/Edit.svg) y ![Editar](/help/assets/icons/Edit.svg) **[!UICONTROL Edit data]** del menú contextual.

  1. En el diálogo **[!UICONTROL Edit Data]**:

     1. Seleccione una métrica de **[!UICONTROL Select a metric]**, por ejemplo **[!UICONTROL Impressions]**.
     1. Seleccione una categoría de **[!UICONTROL Select category]**, por ejemplo **[!UICONTROL Media types]**.
     1. (opcional) seleccione una segunda categoría de **[!UICONTROL Select second category (optional)]**, por ejemplo **[!UICONTROL Traffic sources]**.
     1. Seleccione ![Reloj](/help/assets/icons/Clock.svg) **[!UICONTROL Time]** o ![Calculadora](/help/assets/icons/Calculator.svg) **[!UICONTROL Total]** como tipo de análisis en **[!UICONTROL Select analysis type]**.

        Si selecciona ![Reloj](/help/assets/icons/Clock.svg) **[!UICONTROL Time]**, puede especificar la frecuencia de tiempo. Seleccione **[!UICONTROL Daily]**, **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]** o **[!UICONTROL Quarterly]** de **[!UICONTROL Select time frequency]**.

        Verá una vista previa actualizada de su selección actual en [!UICONTROL Preview Area] y de su visualización actual debajo de [!UICONTROL Current].

        ![Editar widget de datos armonizados](/help/assets/edit-harmonized-data-widget.png)

        Si no se puede procesar la vista previa porque no hay datos disponibles, verá ![Error de datos](/help/assets/icons/DataUnavailable.svg) [!UICONTROL Insights Not Available] - [!UICONTROL Harmonized fields are not available].

     1. Seleccione **[!UICONTROL Apply]** para aplicar los cambios a la visualización. Seleccione **[!UICONTROL Cancel]** para cancelar los cambios realizados en la visualización actual.
