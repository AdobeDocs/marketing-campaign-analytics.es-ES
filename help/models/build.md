---
title: Modelos De Compilación En Marketing Campaign Analytics
description: Obtenga información sobre cómo crear modelos en Marketing Campaign Analytics, incluido cómo configurar y especificar opciones avanzadas para el modelo. Como objetivos de conversión, puntos de contacto, stock de anuncios y programación.
feature: Models
solution: Marketing Campaign Analytics
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
TQID: 'https://experienceleague.adobe.com/cFNaPV6-R3d5ogcBfOyEVNqJoIvfg2JBzVeedjrtEq4'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Marketing Campaign Analytics
feature_v2:
  - id: e0abf868-dae2-4c1c-83e9-b21799232845
    internal-label: Datasets
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
    internal-label: Models
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized data
subfeature_v2:
  - id: a9505d76-24a1-4ffe-bd01-6ac32d5af453
    internal-label: Model insights
  - id: bc2f5225-03d4-4bc8-89ec-99d78c30e6dd
    internal-label: Conversions
  - id: c89e26b6-808d-4500-8b01-450a63466999
    internal-label: Build model
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
    internal-label: Email marketing
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 1e187d334357fc2696b7a15796d669f9632b63cb
workflow-type: tm+mt
source-wordcount: '2134'
ht-degree: 8%
---
# Modelos de compilación

{{mm-mca-rebranding}}

Para crear sus modelos personalizados con tecnología de IA, la interfaz proporciona un flujo de configuración de modelo guiado paso a paso.

En la interfaz de ![Modelos](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** en [!DNL Marketing Campaign Analytics], seleccione **[!UICONTROL Open model canvas]**.

## Configuración

Usted define un nombre y una descripción en el paso **[!UICONTROL Setup]**:

1. Escriba el modelo **[!UICONTROL Name]**, por ejemplo `Demo model`. Escriba un **[!UICONTROL Description]**, por ejemplo `Demo model to explore AI features of Marketing Campaign Analytics`.

   ![Nombre y descripción del modelo](/help/assets/model-name-description.png)

1. Seleccione **[!UICONTROL Next]** para continuar con el paso siguiente. Seleccione **[!UICONTROL Cancel]** para cancelar la configuración del modelo.

## Configurar {#configure}

>[!CONTEXTUALHELP]
>id="model_marketingtouchpoints_select"
>title="Puntos de contacto de marketing"
>abstract="Los puntos de contacto de marketing son eventos de marketing a nivel de destinatario, individuales o de cookie que se utilizan para evaluar el impacto de las inversiones de marketing en las conversiones numéricas o basadas en ingresos.<br/><br/>No puede configurar el modelo con puntos de contacto que tengan datos superpuestos y debe haber al menos un punto de contacto con gasto."


El modelo se configura en el paso **[!UICONTROL Configure]**. La configuración implica la activación del modelado funnel completo, la definición de los objetivos de conversión, los puntos de contacto de marketing, la población de datos apta, los factores externos e internos, etc.

1. Si desea habilitar [modelado funnel completo](./overview.md#full-funnel-modeling), en la sección **[!UICONTROL Full funnel model]**:

   1. Seleccione **[!UICONTROL Enable full funnel modeling]**.
   1. Seleccione una conversión superior en el menú desplegable **[!UICONTROL Upper funnel conversion]**.

1. En la sección **[!UICONTROL Conversion goal]**:

   ![Modelo: paso de conversión](/help/assets/model-conversion-step.png)

   1. Seleccione una conversión en el menú desplegable **[!UICONTROL Conversion]**. Las conversiones disponibles son las que definió como parte de [Conversiones](../harmonize-data/conversions.md) en [!UICONTROL Harmonized datasets]. Por ejemplo, **[!UICONTROL Online Conversion]**.

   1. Puede seleccionar ![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a conversion]** para crear una conversión directamente desde la configuración del modelo.



1. En la sección **[!UICONTROL Marketing touchpoints]**, puede seleccionar uno o más puntos de contacto de marketing, correspondientes a los puntos de contacto de marketing que definió como parte de [puntos de contacto de marketing](../harmonize-data/marketing-touchpoints.md) en [!UICONTROL Harmonized datasets].


   ![Modelo: paso de punto de contacto de marketing](/help/assets/model-marketing-touchpoint-step.png)

   1. Seleccione uno o más puntos de contacto de marketing en el menú desplegable **[!UICONTROL Touchpoint include]**.

      * Puede usar ![CrossSize75](/help/assets/icons/CrossSize75.svg) para quitar un punto de contacto.
      * Puede usar **[!UICONTROL Clear all]** para eliminar todos los puntos de contacto.

   1. Puede seleccionar ![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a touchpoint]** para crear un punto de contacto de marketing directamente desde la configuración del modelo.

   >[!NOTE]
   >
   >No puede configurar el modelo con puntos de contacto que tengan datos superpuestos y debe haber al menos un punto de contacto con gasto.

1. De forma predeterminada, se genera una puntuación para todos los datos de la vista armonizada. Para puntuar solo un subconjunto de la población, defina uno o más filtros usando contenedores en la sección **[!UICONTROL Eligible data population]**.

   ![Modelo: población de datos elegible](/help/assets/model-eligible-data-population-step.png)

   * Para cada contenedor, defina uno o más eventos.

     1. Para cada evento:

        1. Seleccione una métrica o dimensión de **[!UICONTROL _Seleccionar campo armonizado_]**.

        1. Seleccione el operador apropiado: **[!UICONTROL equals]**, **[!UICONTROL not equals]**, **[!UICONTROL less than]**, **[!UICONTROL greater than]**, **[!UICONTROL starts with]**, **[!UICONTROL doesn't start with]**, **[!UICONTROL ends with]**, **[!UICONTROL doesn't end with]**, **[!UICONTROL contains]**, **[!UICONTROL doesn't contain]**, **[!UICONTROL is in]** o **[!UICONTROL is not in]**.

        1. Escriba o seleccione un valor en **[!UICONTROL _Escriba o seleccione el valor_]**.

     1. Para agregar un evento adicional en el contenedor, seleccione ![Agregar](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add event]**.

     1. Para quitar un evento del contenedor, seleccione ![Cerrar](/help/assets/icons/CrossSize75.svg).

     1. Para filtrar usando todos o cualquiera de los múltiples eventos definidos en el contenedor, seleccione **[!UICONTROL Any of]** o **[!UICONTROL All of]**. La etiqueta cambia de **[!UICONTROL Include ... Or ...]** a **[!UICONTROL Include ... And ...]**.

   * Para agregar un contenedor de población de datos apto, seleccione ![Agregar](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add eligible population]**.

   * Para quitar un contenedor de población de datos apto, dentro del contenedor, seleccione ![Más](/help/assets/icons/More.svg) y **[!UICONTROL Remove container]** en el menú contextual.

   * Seleccione **And** y **Or** entre contenedores para generar definiciones más complejas para la población de datos elegible.

1. Puede administrar conjuntos de datos que contengan factores internos o externos en la sección **[!UICONTROL Factor]**.

   * Para agregar un conjunto de datos de factor, seleccione **[!UICONTROL Add Factor]**. Puede agregar un máximo de 30 factores a un modelo.

     ![Modelo - Paso de factor](../assets/model-factors-dataset-step.png)

     1. Seleccione un(a) **[!UICONTROL Factor dataset]** del menú desplegable. Los factores disponibles son los factores para los que ha definido un campo armonizado en [reglas del conjunto de datos](/help/harmonize-data/dataset-rules.md#create-a-dataset-rule).

        En función del conjunto de datos seleccionado, **[!UICONTROL Factor type]** es **[!UICONTROL Internal]** o **[!UICONTROL External]**.

     1. Seleccione **[!UICONTROL Impact on conversion]** del menú desplegable. Las opciones disponibles son: **[!UICONTROL Auto]**, **[!UICONTROL Positive]** o **[!UICONTROL Negative]**. La opción predeterminada es **[!UICONTROL Auto]**, que permite al modelo determinar el impacto del conjunto de datos de factor.

   * Para eliminar un conjunto de datos de factor, seleccione ![CrossSize200](/help/assets/icons/CrossSize400.svg).

   * Si el modelo está habilitado para [modelado funnel completo](./overview.md#full-funnel-modeling), debe definir relaciones causales y relaciones causales de factor para los factores que agregue al modelo.

     ![Modelo - Paso de factor funnel](../assets/model-factors-dataset-step-funnel.png)

     * Para definir relaciones causales, en la tabla **[!UICONTROL Causal relationship]** s, seleccione ![SelectBox](/help/assets/icons/SelectBox.svg) para cada canal (**[!UICONTROL Source]**) para indicar si el canal influye en los KPI de conversión superior e inferior.

       Puede seleccionar ![SelectBox](/help/assets/icons/SelectBox.svg) el encabezado de columna para el KPI de conversión superior y el KPI de conversión inferior para definir rápidamente que todos los canales influyen en el KPI.

     * Cuando haya definido factores, defina las relaciones causales de los factores. Para definir las relaciones causales del factor, en la tabla **[!UICONTROL Factor causal relationships]**, seleccione ![SelectBox](/help/assets/icons/SelectBox.svg) para cada factor (**[!UICONTROL Factor]**) para indicar si el factor influye en los KPI de conversión superior e inferior.

       Puede seleccionar ![SelectBox](/help/assets/icons/SelectBox.svg) el encabezado de columna para el KPI de conversión superior y el KPI de conversión inferior para definir rápidamente que todos los factores influyen en el KPI.


1. Para definir la ventana retrospectiva del modelo, escriba un valor entre `1` y `52` en **[!UICONTROL Give contribution credit to touchpoints occurring within]**... **[!UICONTROL weeks prior to the conversion]** en la sección **[!UICONTROL Define lookback window]**.

   Si el modelo está habilitado para [modelado funnel completo](./overview.md#full-funnel-modeling):

   * Para definir la ventana retrospectiva para funnel inferior, escriba un valor entre `1` y `52` en **[!UICONTROL Give contribution credit to touchpoints occurring within]**... **[!UICONTROL weeks prior to the conversion]** para **[!UICONTROL Lower funnel]** en la sección **[!UICONTROL Define lookback window]**.

   * Para definir la ventana retrospectiva para la funnel superior, escriba un valor entre `1` y `52` en **[!UICONTROL Give contribution credit to touchpoints occurring within]**... **[!UICONTROL weeks prior to the upper funnel conversion]** para **[!UICONTROL Upper funnel]** en la sección **[!UICONTROL Define lookback window]**.


1. Para definir la ventana de formación de un modelo, en **[!UICONTROL Define training window]**, seleccione dónde iniciar las conversiones de puntuación.

   ![Modelo - Definir ventana de formación](/help/assets/model-define-training-window.png)

   Puede seleccionar entre:

   * **[!UICONTROL Have Marketing Campaign Analytics select a helpful training window]** y

   * **[!UICONTROL Manually input a training window]**. Cuando esté seleccionado, defina el número de años en **[!UICONTROL Include events the following years prior to a conversion]**.

   Esta entrada es necesaria para un modelo. La cantidad de años determina cómo se limita el canal y el stock, que puede configurar en el paso **[!UICONTROL Advanced]**.

1. Seleccione **[!UICONTROL Next]** para continuar con el paso siguiente. Si se necesita más configuración, un contorno rojo y texto explican qué configuración adicional se requiere. <br/>Seleccione **[!UICONTROL Back]** para regresar al paso anterior. <br/>Seleccione **[!UICONTROL Cancel]** para cancelar la configuración del modelo.


## Avanzadas {#advanced}

>[!CONTEXTUALHELP]
>id="model_advanced_channeladstock"
>title="Adstock del canal"
>abstract="Incorpore experiencia del dominio, resultados de la experimentación o análisis de canal anteriores directamente en la configuración del modelo. La configuración del Adstock ayuda a guiar el modelo para que se ajuste a las expectativas del mundo real y mejora la interpretabilidad y la confianza en el resultado. El total de semanas de retrospectiva más semanas de retardo por canal se limita a una octava parte de la ventana de formación configurada. Este límite permite que el modelo disponga de datos suficientes para conocer los efectos del Adstock."

Puede especificar la configuración avanzada en el paso **[!UICONTROL Advanced]**. En este paso, puede definir [gasto compartido](#spend-share), habilitar el modelo para [atribución multitáctil (MTA)](#mta), definir [conocimiento previo](#prior-knowledge) y definir [canal y stock](#channel-adstock).

### Gasto compartido

En la sección **[!UICONTROL Spend share]**:

* Para usar las relaciones de inversión de marketing históricas para informar al modelo cuando los datos de marketing son dispersos, active **[!UICONTROL Allow spend share]**.

  Si el modelo está habilitado para [modelado funnel completo](./overview.md#full-funnel-modeling):

  * Para usar las relaciones de inversión de marketing históricas para informar al modelo cuando los datos de marketing son dispersos, active **[!UICONTROL Allow spend share for the lower funnel]**.
  * Para usar las relaciones de inversión de marketing históricas para informar al modelo cuando los datos de marketing son dispersos, active **[!UICONTROL Allow spend share for the upper funnel]**.

* Se recomienda esta configuración, especialmente en los siguientes casos:
  * Un canal no tiene suficientes observaciones (por ejemplo, baja frecuencia de gasto, impresiones o clics).
  * Está modelando medios puntiagudos pero regulares y potencialmente de alto gasto (como TV para algunas marcas), donde los datos son escasos.

  >[!NOTE]
  >
  >Para inversiones puntuales (por ejemplo, un anuncio de la Super Bowl), incorpore esos datos como un factor en lugar de depender de la cuota de gasto.
  >



### MTA

En la sección **[!UICONTROL MTA enabled]**:

* Para habilitar las características de MTA para el modelo, active **[!UICONTROL MTA enabled]**. Si ha habilitado el MTA, las perspectivas de atribución multitáctil están disponibles después de haber entrenado y puntuado al modelo. Consulte la pestaña [Atribución](insights.md#attribution) en [Información del modelo](insights.md).


### Conocimientos previos

En la sección **[!UICONTROL Prior knowledge]**:

![Modelo - Conocimientos previos](/help/assets/model-prior-knowledge-step.png)

1. Seleccione **[!UICONTROL Rule type]**, que es de forma predeterminada **[!UICONTROL Absolute values]**.

1. Si el modelo está habilitado para [modelado funnel completo](./overview.md#full-funnel-modeling):

   * Seleccione **[!UICONTROL Lower funnel]** o **[!UICONTROL Upper funnel]** de **[!UICONTROL Select metric]** como métrica de funnel que se utilizará para el conocimiento previo.

1. Especifique los porcentajes de contribución para cualquiera de los canales enumerados en **[!UICONTROL Name]**, utilizando la columna **[!UICONTROL Contribution proportion]**.

1. Si corresponde, puede agregar para cada canal un porcentaje de **[!UICONTROL Level of confidence]**.

1. Si es necesario, use **[!UICONTROL Clear all]** para borrar todos los valores de entrada de las columnas **[!UICONTROL Contribution proportion]** y **[!UICONTROL Level of confidence]**.


### Adstock del canal

En la sección **[!UICONTROL Channel adstock]** puede definir retrospectivas de stock individuales (efectos de arrastre o deterioro) y un retardo (tiempo de respuesta demorado) para cada canal (canal de marketing) que haya definido en su modelo.

Esta configuración de stock de anuncios de canal permite un control detallado sobre cómo los distintos canales de marketing afectan a los resultados empresariales a lo largo del tiempo. También puede utilizar valores por defecto del sistema y una configuración estándar.

La configuración de canal de anuncios le ayuda a capturar matices específicos del canal. Por ejemplo, el impacto a largo plazo de las campañas de TV, el impacto a corto plazo de la búsqueda de pago o el desfase entre el gasto de los influenciadores y las conversiones observables. Experimente con los parámetros de retardo y retrospectiva de AdStock para generar perspectivas más precisas, personalizadas y fiables. En última instancia, la configuración de un canal y un stock puede dar lugar a asignaciones presupuestarias más precisas y mejores decisiones empresariales.

![Adstock de canal](/help/assets/channel-ad-stock.png)

Para configurar un archivo de canal:

* Si el modelo está habilitado para [modelado funnel completo](./overview.md#full-funnel-modeling), seleccione **[!UICONTROL Lower funnel]** o **[!UICONTROL Upper funnel]** de **[!UICONTROL Select metric]** como métrica de funnel que se usará para el inventario de anuncios de canal.

* Para cada canal (**[!UICONTROL Name]**), defina un valor **[!UICONTROL Lag (weeks)]**, un valor **[!UICONTROL Min Lookback (weeks)]** y **[!UICONTROL Max Lookback (weeks)]**. Para cada valor:

  * Para aumentar un valor, use ![Agregar](/help/assets/icons/Add.svg); para reducirlo, use ![Restar](/help/assets/icons/Subtract.svg); o escriba un valor manualmente.

  El total de semanas de retraso más las semanas de retrospectiva máximas por canal se limita a una octava parte de la ventana de formación configurada. Este límite permite que el modelo disponga de datos suficientes para conocer los efectos del Adstock. Por ejemplo, para una ventana de formación de dos años, el máximo de **[!UICONTROL Lag (weeks)]** y **[!UICONTROL Lookback (weeks)]** para un canal es de 13 semanas. Este límite se impone al definir los valores.

* Para restablecer todos los valores predeterminados de los anuncios de canal:

  * Seleccione **[!UICONTROL Reset to defaults]**.


## Definir opciones

Puede [programar entrenamiento y puntuación](#schedule), y especificar [campos granulares de informe de perspectivas](#granular-insights-reporting-fields) para su modelo en el paso **[!UICONTROL Set options]**.


### Programación

En la sección **[!UICONTROL Schedule]**, puede programar la formación y la puntuación del modelo.

![Modelo de horario](../assets/model-schedule.png)

Para programar la puntuación y la formación del modelo:

1. Activar **[!UICONTROL Enable scheduled model scoring and training]**.
1. Seleccionar un **[!UICONTROL Scoring frequency]**:

   * **[!UICONTROL Daily]**: escriba una hora válida (por ejemplo, `05:22 pm`) o use ![Reloj](/help/assets/icons/Clock.svg) para definir la hora.
   * **[!UICONTROL Weekly]**: seleccione un día de la semana e introduzca una hora válida (por ejemplo, `05:22 pm`) o use ![Reloj](/help/assets/icons/Clock.svg) para definir la hora.
   * **[!UICONTROL Monthly]**: seleccione un día del mes en el menú desplegable Ejecutar en cada e introduzca una hora válida (por ejemplo, `05:22 pm`) o use ![Reloj](/help/assets/icons/Clock.svg) para definir la hora.

1. Seleccione un(a) **[!UICONTROL Training frequency]** del menú desplegable: **[!UICONTROL Monthly]**, **[!UICONTROL Quarterly]**, **[!UICONTROL Yearly]** o **[!UICONTROL None]**.


### Customer Journey Analytics {#cja}

>[!CONTEXTUALHELP]
>id="model_enable_cja"
>title="Habilitar Customer Journey Analytics"
>abstract="Para que los datos de puntuación estén disponibles para informes y análisis en Customer Journey Analytics, habilite esta configuración. Una vez activado, debe eliminar el modelo para desactivar esta configuración."

{{release-limited-testing-section}}

Si tiene derecho a Customer Journey Analytics y ha creado una o más [reglas de conjuntos de datos](/help/harmonize-data/dataset-rules.md) para Marketing Campaign Analytics en una zona protegida concreta:

* Se crean dos conjuntos de datos de Marketing Campaign Analytics dedicados en su zona protegida de Experience Platform.
* Se crea una conexión [connection](https://experienceleague.adobe.com/es/docs/analytics-platform/using/cja-connections/overview) de Customer Journey Analytics con el título **[!UICONTROL Marketing Campaign Analytics Enabled Connection (_sandbox-name _)]**&#x200B;que contiene los conjuntos de datos de Marketing Campaign Analytics dedicados.
* Se crea una [vista de datos](https://experienceleague.adobe.com/es/docs/analytics-platform/using/cja-dataviews/data-views) de Customer Journey Analytics, con el título **[!UICONTROL Marketing Campaign Analytics Insights Data View (_sandbox-name _)]**, basada en la conexión.

Tanto la conexión como la vista de datos son propiedad del sistema. No puede actualizar ni eliminar la conexión o la vista de datos.

Para que los datos de puntuación del modelo estén disponibles para Customer Journey Analytics a través de los conjuntos de datos, la conexión y la vista de datos mencionados anteriormente:

* Seleccione **[!UICONTROL Enable scores for Customer Journey Analytics]**.

  Una vez habilitada esta opción, solo se puede deshabilitar eliminando el modelo.

Para informar y analizar los datos de Marketing Campaign Analytics rápidamente, en un [proyecto del espacio de trabajo](https://experienceleague.adobe.com/es/docs/analytics-platform/using/cja-workspace/home) de Customer Journey Analytics:

1. Seleccione **[!UICONTROL Workspace]** > **[!UICONTROL Adobe templates]**.
1. Seleccione la **[!UICONTROL Marketing Campaign Analytics Insights Data View (_sandbox-name _)]**&#x200B;dedicada como la vista de datos que se utilizará para un proyecto.
1. Seleccione **[!UICONTROL Marketing Campaign Analytics Incremental Insights]** [plantilla](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/templates/use-templates#marketing-campaign-analytics-templates).
   * Seleccione **[!UICONTROL Preview]** para ver una vista previa.

     ![Vista previa de la plantilla Marketing Campaign Analytics](/help/assets/model-cja-enable-template.png)
   * Seleccione **[!UICONTROL Use template]** para crear un proyecto basado en la plantilla.

### Campos de informes de perspectivas granulares

La sección **[!UICONTROL Granular insights reporting fields]** utiliza la funcionalidad de informes de incrementalidad granular. Esta funcionalidad le permite seleccionar campos armonizados para desglosar las puntuaciones de incrementalidad de conversión y puntos de contacto.

![Definir campos granulares de informes de perspectivas](/help/assets/granular-insights-reporting-fields.png)

Estos campos armonizados se definen de modo que se pueda explorar en profundidad el sistema de informes del modelo mediante columnas de informes granulares en lugar de tener que crear modelos separados.

Por ejemplo, crea un modelo centrado en los ingresos, pero también le interesa el rendimiento de la campaña, el tipo de medio, la región y las fuentes de tráfico. Sin la funcionalidad de creación de informes de incrementalidad granular, debe crear cuatro modelos independientes. Con la funcionalidad de creación de informes de incrementalidad granular, puede desglosar el modelo de ingresos en campañas, tipos de medios, regiones y fuentes de tráfico.

1. Seleccione uno o más campos armonizados de **[!UICONTROL _Seleccionar campos armonizados_]** debajo de **[!UICONTROL Includes]**. Los campos armonizados seleccionados se añaden al panel.
1. Seleccione **[!UICONTROL *Campo armonizado *]**![CrossSize100](/help/assets/icons/CrossSize100.svg) para quitar un campo armonizado del contenedor con los campos armonizados seleccionados.
1. Seleccione **[!UICONTROL Clear all]** para eliminar todos los campos armonizados seleccionados.

Los campos armonizados seleccionados para los informes de incrementalidad granular están disponibles como parte de los conjuntos de datos [schema](/help/ingest-data/schemas.md) y [dataset](/help/ingest-data/datasets.md) de Experience Platform que resultan de la puntuación del modelo. Los campos de informes de datos detallados se pueden encontrar dentro de los objetos **[!UICONTROL conversionPassthrough]** y **[!UICONTROL touchpointPassthrough]**.

![Captura de pantalla de los objetos conversionPassthrough y touchpointPassthrough en un esquema para un modelo habilitado para la creación de informes de incrementalidad granular](/help/assets/schema-granular-insights-reporting.png)


## Finalizar

* Seleccione **[!UICONTROL Finish]** para finalizar la configuración del modelo.

  * En el cuadro de diálogo **[!UICONTROL Create instance?]**, seleccione **[!UICONTROL Ok]** para almacenar en déclencheur el primer conjunto de entrenamientos y ejecuciones de puntuación inmediatamente. Su modelo aparece con el estado ![StatusOrange](/help/assets/icons/StatusOrange.svg) **[!UICONTROL Awaiting training]**.

    Seleccione **[!UICONTROL Cancel]** para cancelar.

  * Si se necesita más configuración, un contorno rojo y texto explican qué configuración adicional se requiere.

* Seleccione **[!UICONTROL Back]** para volver al paso anterior.

* Seleccione **[!UICONTROL Cancel]** para cancelar la configuración del modelo.

