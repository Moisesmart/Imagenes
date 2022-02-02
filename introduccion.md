# ¿Qué es Helm? ¿Qué son los charts? 


# **Helm**
## Helm (del término marítimo de timón) es una herramienta para gestionar aplicaciones de Kubernetes. Helm te ayuda a timonear Kubernetes usando cartas de navegación, que en inglés se conocen como Helm Charts. Aunque nos gustan las referencias de marítimas de Helm y Kubernetes, el término ‘carta de navegación’ o ‘carta’ puede ser más difícil de entender que Chart.

La principal función de Helm es definir, instalar y actualizar aplicaciones complejas de Kubernetes. Helm es mantenido por la CNCF en colaboración con Microsoft, Google, Bitnami y la comunidad de Helm.


# **Charts** 

## Con Helm Charts es posible crear, versionar y publicar una aplicación Kubernetes. Cuando usamos Helm Charts tenemos un asistente de optimización que facilita la administración e instalación de las aplicaciones Kubernetes y el proceso de empaquetamiento.

## Helm Charts se divide en dos vertientes: una parte es Helm, como cliente y la otra es Tiller como servidor.


## **Vertientes**

### Tiller - servidor de Helm

### Tiller es el componente que se encarga de la gestión de los Charts, específicamente en sus instalaciones. Interactúa directamente con el API de Kubernetes para instalar, actualizar, consultar y eliminar recursos Kubernetes. También almacena los objetos de cada release o distribución.
Helm - el cliente

### Por su parte, Helm se ejecuta directamente en un equipo o en el dispositivo elegido para la ejecución. Los paquetes Helm están compuestos de una descripción del paquete y de archivos contenedores de manifiestos Kubernetes.
