# 📦 PackAlert: Sistema de Gestión Logístico en Tiempo Real
>**⚠️ Nota de Confidencialidad:** *Este sistema fue desarrollado por iniciativa propia y es propiedad intelectual del autor. Dado que es una herramienta operativa especifica para un cliente, el codigo fuente no es público en este repositorio. Acontinuación, se presenta una demostración técnica y la arquitectura del Sistema.*
>
>--
>## 🛑 El Problema (Antes de PackAlert)
>La empresa enfrentaba una desconexion crítica entre area de facturación(oficina) y el área de empaquetado (bodega), generando los siguientes problemas operativos:
>
>1. **Tiempos Muertos:** En varios casos, al revisar inicialmente no se encontra paquetería disponible, pero más tarde aparecen paquetes nuevos sin previo aviso.
>2. **Falta de comunicación:** No existía una comunicación clara ni en tiempo real que indicara cuándo había nueva paquetería lista para empacar.
>3. **Sobrecostos:** En días de alta carga laboral, esta desorganización obligaba a realizar horas extras y retrasaba la salida de los pedidos.
>4. **Errores Operativos:** La falta de un sistema de aviso provoca desorganización.
>
>   ✅ La solución Desarrollada
>Diseñé y programé **PackAlert**, una aplicación de escritorio cliente-servidor que funciona en la red local (LAN) y elimina la necesidad de verificaciones manuales.
>
>### ¿Cómo funciona?
>1. **Oficina:** El operador ingresa el pedido listo.
>2. **Transmisión:** El servidor procesa el dato y lo envía en milisegundos a la bodega.
>3. **Bodega:** Recibe una **Notificación Visual y Sonora** (nativa de Windows) y el pedido se agrega automáticamente a una "Lista de Pendientes" en pantalla.
>
>
## 🔧 Tecnologías Utilizadas
* **Lenguaje:** Python 3.12
* **Comunicación:** WebSockets (SocketIO + Eventlet) para tiempo real.
* **Redes:** Protocolo UDP Broadcast (Auto-descubrimiento de servidores sin configurar IPs).
* **Persistencia:** Generación automática de reportes en Excel (.csv) para auditoría.
* **Despliegue:** Empaquetado en `.exe` (PyInstaller) para fácil instalación en PCs sin Python.

## 🚀 Impacto del Proyecto
* **Redujcción de tiempos:** Eliminación de las caminatas innecesarias para verificar pedidos.
* **Organización:** La bodega ahora puede filtrar pedidos por "Tienda" específica.
* **Cero Dependencia:** El sistema funciona 100% Offline (Sin internet), solo requiere red local.

---
*Desarrollado por: Juan Esteban Palacio Osorio*









