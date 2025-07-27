# 🚚 Automatización y Análisis Logístico

Este proyecto integral combina **Power BI** para el análisis y **Python** para la automatización, monitoreando las solicitudes de montacargas en operaciones de almacén/logística.

**Aclaración Importante:** Desarrollado con **datos reales** operativos. Por motivos de confidencialidad, las capturas de pantalla del dashboard han sido **censuradas** para su presentación pública. El objetivo es mostrar la metodología y las capacidades técnicas.

---

## 🔍 Contexto y Propósito

El objetivo fue optimizar la gestión y el seguimiento de solicitudes de montacargas. Permite a la gerencia monitorear la eficiencia, el volumen de solicitudes y paletas trasladadas, así como evaluar el rendimiento del personal, todo a través de un flujo de información automatizado y en tiempo casi real.

---

## 🛠️ Herramientas y Tecnologías

* **Power BI Desktop:** Modelado de datos, visualizaciones interactivas y diseño del dashboard.
* **DAX:** Creación de KPIs avanzados y medidas complejas.
* **Python:** Desarrollo del script de automatización (`Selenium` para extracción web, `Plyer` para notificaciones).
* **Microsoft Power Apps & Lists (SharePoint):** Origen de los datos de solicitud.
* **Power BI Service / Microsoft Fabric:** Publicación y actualización automática del dashboard.
* **Programador de Tareas (Windows Task Scheduler):** Para la orquestación automática del script Python.

---

## 🚀 Flujo de Datos Automatizado

Los datos provienen de registros operativos reales y siguen un flujo completamente automatizado:
1.  Las solicitudes se generan en **Power Apps** y se almacenan en una **Microsoft List (SharePoint)**.
2.  Un script de **Python** (`Selenium`) automatiza la descarga periódica (cada 29 minutos) del archivo CSV con estos datos.
3.  El dashboard de **Power BI** se alimenta de esta fuente y se actualiza automáticamente cada 30 minutos en **Power BI Service**, garantizando información siempre al día.

![Fragmento del Script Python de Automatización](./script_automatizacion_montacargas.jpg)

---

## 📊 Vistas Clave del Dashboard

Aquí se presenta la vista principal del dashboard interactivo:

### Dashboard Principal de Solicitudes de Montacargas

Ofrece una visión general de solicitudes, paletas trasladadas, estatus de prioridad, rendimiento por usuario y tendencias temporales.

![Dashboard de Solicitudes de Montacargas (Datos Censurados)](./dashboard_montacargas_general.png)

---

## 💡 Impacto y Valor Aportado

* **Eficiencia Operativa:** Identificación de cuellos de botella y optimización en la asignación de recursos de montacargas.
* **Decisiones en Tiempo Real:** Acceso a información actualizada para una gestión más ágil y efectiva.
* **Automatización Robusta:** Reducción drástica del trabajo manual y mejora en la frescura de los datos.

---

## 🧑‍💼 Autor

**Renato Cobeñas** 📧 rencou4@gmail.com
[LinkedIn](https://www.linkedin.com/in/tuusuario)
[GitHub](https://github.com/RenCoU4)
