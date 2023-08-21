# Cloud Computing: Trabajo de Investigación


## 1. VM en Proovedores líderes de Cloud Computing

### 1.1 Regiones y Zonas de disponibilidad o equivalente.

Una **región** es una ubicación física geográfica, donde se encuentran zonas de disponibilidad que albergan centro de datos ó **data centers** de algún proveedor de Cloud Computing. En una región pueden existir muchas zonas de disponibilidad (**Availability Zone**), pero como mínimo se espera que 3, pues si una de estas **AZ** llega a caerse existe un respaldo de conexión en la misma región (**Zone-Redundant**). 

#### 1.1.1 AWS

Según su propio sitio web, dentro de la sección [global infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/), se determina que al momento de redactar este trabajo de investigación, **Amazon Web Services** cuenta con 102 zonas de disponibilidad (*availability zone*) dentro de 32 regiones alrededor del mundo.

#### 1.1.2 Microsoft Azure

Azure cuenta con un apartado de documentación, tutoriales y guías donde fue posible hallar las regiones y zonas de disponibilidad de las cuales brindan sus servicios. No obstante guiándome de su apartado [learn.microsoft](https://learn.microsoft.com/en-us/azure/reliability/availability-zones-service-support) y su apartado interactivo web [Azure geographies](https://azure.microsoft.com/en-us/explore/global-infrastructure/geographies/#overview), podemos decir que Azure cuenta con soporte para más de 60 regiones.

No se menciona oficialmente pero considerando la premisa de Azure por otorgar como mínimo 3 zonas de disponibilidad, entonces estaríamos hablando de como mínimo $60 \cdot 3 \approx 120$ zonas de disponibilidad a su cargo. 

#### 1.1.3 Google Cloud

El gigante de Google anuncia en su sitio web [google cloud](https://cloud.google.com/about/locations?hl=es) que cuenta hasta la fecha con 37 regiones y 112 zonas de disponibilidad. No obstante en su mismo sitio prometen que están trabajando para extenderse a 11 nuevas zonas.

### 1.2 Precios para Máquinas Virtuales

### 1.3 Comparación entre los 3 proveedores. Máquinas pequeñas/medianas/grandes.

### 1.4 Imágenes y diagramas

### 1.5 Referencias APA

- https://azure.microsoft.com/es-es/explore/global-infrastructure
- https://aws.amazon.com/about-aws/global-infrastructure/

---

## 2. Caso de evaluación de costos de VM

La Organización de las Naciones Unidas (ONU) desea procesar los datos de censos de población y vivienda de cada uno de sus 193 países miembro para poder establecer un mapa de pobreza mundial y poder brindar ayuda de salud y humanitaria en el futuro. Por política de privacidad de datos, la ONU le pide que las máquinas virtuales se sitúen en Europa.

La ONU necesita una gran potencia de computación por 90 días y su equipo técnico ha estimado lo siguiente:

- 80 máquinas virtuales Linux cada una con 2 CPU y 4 GB de RAM y 20 GB de disco SSD de HW como mínimo para hacer los cálculos.
- 10 máquinas virtuales Linux cada una con 4 CPU y 8 GB de RAM y 500 GB de disco SSD de HW como mínimo para la base de datos.

### 2.1 Región para cada proveedor y argumentar elección

### 2.2 Tamaño de máquinas virtuales más adecuado para cada proveedor

### 2.3 Calcular costos de Compute y Storage.

### 2.4 Recomendación de proveedor

### 2.5 Imágenes y Diagramas

### 2.6 Referencias APA