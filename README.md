# 📦 Código Fuente: Servidor Odoo 19 (Proyecto ERP)

Este repositorio almacena todo el código fuente y las configuraciones de nuestro servidor **Odoo 19**. Es el resultado de un proyecto práctico de clase donde montamos y personalizamos un sistema ERP distribuido para gestionar dos negocios distintos de forma simultánea.

## 📂 ¿Qué contiene este repositorio?

Aquí encontrarás la estructura completa de nuestro servidor, incluyendo las configuraciones del sistema, los módulos nativos, los añadidos de terceros y las modificaciones visuales que fuimos haciendo durante el desarrollo. Básicamente, es el "cerebro" de nuestro proyecto.

Entre los archivos destacables se encuentran:
* El archivo `odoo.conf` con las rutas personalizadas (como la gestión de los logs).
* La carpeta de `addons` con módulos extra que no vienen por defecto.
* Los *assets* e imágenes modificadas del sistema.

## 🏗️ Contexto del Proyecto

Para entender la utilidad de este código, este servidor fue diseñado para funcionar dentro de una red con la siguiente estructura de 4 máquinas (desplegadas en IsardVDI):

* 🖥️ **SRV (Servidor Central):** La máquina (Ubuntu 24.04) que ejecuta **este código** y aloja la base de datos PostgreSQL.
* 🛠️ **DEV1 (Desarrollo):** Un entorno seguro aislado donde probábamos los scripts de Python en PyCharm antes de pasarlos al servidor.
* 👕 **POS1 (Tienda de Ropa):** Un terminal cliente en Ubuntu configurado como el punto de venta de la tienda de ropa.
* 🥖 **POS2 (Horno de Pan):** Un terminal cliente en Windows 11 configurado como la caja registradora de la panadería.



## ⚙️ Personalizaciones Incluidas

Dentro de este código fuente hay varias modificaciones y módulos interesantes que le añadimos al Odoo base:

* ♻️ **Sostenibilidad:** Integración manual del módulo de terceros *"Sustainability Point of Sale"* para añadir funcionalidades eco-friendly a los puntos de venta.
* 🛡️ **Seguridad / Auditoría:** Despliegue del paquete *"Audit Log"* para registrar la actividad de los usuarios y tener trazabilidad en caso de incidentes.
* 🎨 **Toques visuales:** Modificamos las entrañas del código para cambiar imágenes predeterminadas. Por ejemplo, cambiamos el logotipo de BMW que viene por defecto en el módulo "Fleet" por el logo de nuestro instituto.
