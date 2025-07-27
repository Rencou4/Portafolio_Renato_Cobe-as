# 🚚 Análisis y Automatización de Solicitudes de Montacargas

Este proyecto integral presenta un dashboard en Power BI y un flujo de datos automatizado con Python para el monitoreo de solicitudes de uso de montacargas en un entorno de almacén/logística.

**Aclaración Importante:** Este dashboard fue construido utilizando **datos reales** de una operación logística. Por motivos de confidencialidad y protección de datos sensibles, **ciertas secciones del dashboard y la información específica (como nombres de usuarios o ubicaciones exactas) han sido censuradas en las capturas de pantalla** para su presentación pública en este portafolio. El enfoque del proyecto es demostrar la metodología, las habilidades técnicas y el valor del análisis.

---

## 🔍 Contexto y Objetivos del Análisis

El objetivo de este proyecto fue optimizar la gestión y el seguimiento de las solicitudes de montacargas, permitiendo a la gerencia:
* Monitorear la eficiencia y el volumen de solicitudes y paletas trasladadas.
* Analizar el estatus y la prioridad de las solicitudes.
* Evaluar el rendimiento del personal en la ejecución de las tareas.
* Proporcionar un flujo de información automatizado y en tiempo casi real para la toma de decisiones operativas.

---

## 📊 Origen y Procesamiento de Datos

Los datos para este análisis provienen de **registros operativos reales** de solicitudes de montacargas.

El flujo de datos es completamente automatizado:
1.  **Recopilación de Datos:** Los registros de solicitudes se generan a través de una aplicación en Power Apps y se almacenan en una Microsoft List en SharePoint.
2.  **Automatización de Extracción (Python):** Se desarrolló un script de Python que utiliza `Selenium` para automatizar la descarga del archivo CSV con los datos de la lista de SharePoint. Este script también maneja el movimiento del archivo a una ubicación específica para su posterior consumo.
    * Puedes ver un fragmento del código Python utilizado para la automatización aquí:
    ![Fragmento del Script Python de Automatización](./script_automatizacion_montacargas.jpg)
3.  **Orquestación y Frecuencia:** El script de Python se ejecuta **automáticamente cada 29 minutos** mediante el Programador de Tareas de Windows, asegurando una actualización constante de los datos.
4.  **Publicación y Actualización en la Nube:** El dashboard de Power BI se alimenta de esta fuente de datos automatizada y ha sido publicado en Power BI Service (o Microsoft Fabric), con **actualizaciones automáticas del dataset configuradas cada 30 minutos**, garantizando que la información esté siempre al día.

---

## 🛠️ Herramientas y Tecnologías

* **Power BI Desktop:** Modelado de datos (con DAX avanzado), creación de visualizaciones interactivas y diseño del dashboard operativo.
* **DAX (Data Analysis Expressions):** Creación de KPIs avanzados y medidas complejas para el análisis de estatus, prioridades, rendimiento de usuarios y tendencias temporales.
* **Python:** Desarrollo del script de automatización (`Selenium` para web scraping/descarga, `Plyer` para notificaciones).
* **Microsoft Power Apps:** Aplicación front-end de origen de las solicitudes.
* **Microsoft Lists (SharePoint):** Base de datos donde residen los datos operativos.
* **Power BI Service / Microsoft Fabric:** Plataforma para la publicación y automatización de la actualización del dashboard.
* **Programador de Tareas (Windows Task Scheduler):** Para la ejecución programada del script de Python.

---

## 📊 Visualizaciones Clave e Insights Destacados

A continuación, se presenta el dashboard interactivo desarrollado, mostrando los principales KPIs y análisis para la gestión de solicitudes de montacargas:

### Dashboard Principal de Solicitudes de Montacargas

Esta vista proporciona una visión general de las solicitudes realizadas, paletas trasladadas, el estatus de prioridad y el rendimiento por usuario, así como una tendencia temporal de las operaciones.

![Dashboard de Solicitudes de Montacargas (Datos Censurados)](./dashboard_montacargas_general.png)

[Opcional: Si tienes otra captura relevante del dashboard censurado, agrégala aquí]
[Opcional: Si tienes el dashboard publicado online en Power BI Service, puedes agregar:]
🔗 [**Ver Dashboard Interactivo Online (Power BI Service)**](https://app.powerbi.com/view?r=xxxxxxxxxxxxxxxxxx)

---

## 💡 Conclusiones y Valor Aportado

* **Eficiencia Operativa:** El dashboard permite identificar cuellos de botella y patrones en la demanda de montacargas, facilitando una mejor asignación de recursos.
* **Rendimiento del Personal:** La visualización del rendimiento por usuario ayuda a identificar oportunidades de capacitación o reconocimiento.
* **Automatización Robusta:** La implementación de un flujo ETL automatizado con Python y SharePoint reduce la dependencia de procesos manuales, asegura la frescura de los datos y libera tiempo para el análisis estratégico.
* **Decisiones Basadas en Datos:** La solución proporciona a la gerencia acceso a información actualizada y relevante para optimizar la toma de decisiones en tiempo real.

---

## 🧑‍💼 Autor

**Renato Cobeñas** 📧 rencou4@gmail.com
[LinkedIn](https://www.linkedin.com/in/tuusuario)
[GitHub](https://github.com/RenCoU4)
