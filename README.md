# Cloud Computing: Trabajo de Investigación


## 1. VM en Proovedores líderes de Cloud Computing

### 1.1 Regiones y Zonas de disponibilidad o equivalente.

Una **región** es una ubicación física geográfica, donde se encuentran zonas de disponibilidad que albergan centro de datos ó **data centers** de algún proveedor de Cloud Computing. En una región pueden existir muchas zonas de disponibilidad (**Availability Zone**), pero como mínimo se espera que 3, pues si una de estas **AZ** llega a caerse existe un respaldo de conexión en la misma región (**Zone-Redundant**). 

#### 1.1.1 Amazon Web Services

Según su propio sitio web, dentro de la sección [global infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/), se determina que al momento de redactar este trabajo de investigación, **Amazon Web Services** cuenta con 102 zonas de disponibilidad (*availability zone*) dentro de 32 regiones alrededor del mundo.

#### 1.1.2 Microsoft Azure

Azure cuenta con un apartado de documentación, tutoriales y guías donde fue posible hallar las regiones y zonas de disponibilidad de las cuales brindan sus servicios. No obstante guiándome de su apartado [learn.microsoft](https://learn.microsoft.com/en-us/azure/reliability/availability-zones-service-support) y su apartado interactivo web [Azure geographies](https://azure.microsoft.com/en-us/explore/global-infrastructure/geographies/#overview), podemos decir que Azure cuenta con soporte para más de 60 regiones.

No se menciona oficialmente pero considerando la premisa de Azure por otorgar como mínimo 3 zonas de disponibilidad, entonces estaríamos hablando de como mínimo $60 \cdot 3 \approx 120$ zonas de disponibilidad a su cargo. 

#### 1.1.3 Google Cloud

El gigante de Google anuncia en su sitio web [google cloud](https://cloud.google.com/about/locations?hl=es) que cuenta hasta la fecha con 37 regiones y 112 zonas de disponibilidad. No obstante en su mismo sitio prometen que están trabajando para extenderse a 11 nuevas zonas.

### 1.2 Precios para Máquinas Virtuales

En este caso para la búsqueda de precio de cada proveedor vamos a comparar en base al modelo más económico que hemos armado, este contará con 2 vCPU, 2 GB de RAM, 10 GB SSD y su región será la costa este de Estados Unidos (**EAST-US**).

No obstante la máquina virtual tendrá un sistema Linux y usará la distribución de Ubuntu. Además estará dentro de la categoría de **Uso general**.

#### 1.2.1 Amazon Web Services

Para el caso de AWS contamos con diferentes instancias que cumplen con el cometido requerido, no obstante para este caso elegimos la instancia [t3a small](https://aws.amazon.com/ec2/pricing/on-demand/). Tiene un precio de $0.0188\$$ la hora, el problema es que debemos sumarle a ello un almacenamiento del tipo [EBS](https://aws.amazon.com/ebs/pricing/) que cuesta aproximadamente $3.00\$$ mensuales con 10GB.

<p align="center">
    <img align="center" src="src/images/cloud_aws.png"/>
</p>

Es así que el total nos da $(0.0188 \cdot 24 \cdot 30) + 3.00 = 16.54 \$$ dolares mensuales.

#### 1.2.2 Microsoft Azure

Para el caso de Microsoft Azure dentro de su [calculadora](https://azure.microsoft.com/es-es/pricing/calculator/) de precios seleccionamos la instancia [Av2 series v2](https://learn.microsoft.com/en-us/azure/virtual-machines/av2-series). Esta cuesta con un costo aproximado de $0.043\$$ por hora. Es decir esto nos daría un costo aproximado de $31,39$$ mensualmente, además debemos considerar que estamos cotizando con un vCPU menos (*modelo más cercano*).

<p align="center">
    <img align="center" src="src/images/cloud_machine.png"/>
</p>

#### 1.2.3 Google Cloud

En este caso, a partir de su modelo de creación por [calculadora](https://cloud.google.com/products/calculator#id=abf90f35-0d04-4796-91a9-8ee4889cf5cb), pudimos encontrar nuestro modelo planteado anteriormente, el cual nos arrojó un costo aproximado de $13.63\$$ y en conjunto con el almacenamiento SSD de 10GB $1.70 \$$, por lo que el costo final es $15.33 \$$ mensuales, muy parecido al de AWS. 

<p align="center">
    <img align="center" src="src/images/cloud_google.png"/>
</p>

### 1.3 Comparación entre los 3 proveedores. Máquinas pequeñas/medianas/grandes.

#### 1.3.1 Máquinas de Amazon

##### 1.3.1.1 Máquina pequeña

##### 1.3.1.2 Máquina mediana

##### 1.3.1.3 Máquina grande

#### 1.3.2 Máquinas de Microsoft Azure

##### 1.3.2.1 Máquina pequeña

##### 1.3.2.2 Máquina mediana

##### 1.3.2.3 Máquina grande

#### 1.3.3 Máquinas de Google Cloud

##### 1.3.3.1 Máquina pequeña

##### 1.3.3.2 Máquina mediana

##### 1.3.3.3 Máquina grande

### 1.4 Imágenes y diagramas

### 1.5 Referencias APA

- https://azure.microsoft.com/es-es/explore/global-infrastructure
- https://aws.amazon.com/about-aws/global-infrastructure/
- https://cloud.google.com/products/calculator#id=abf90f35-0d04-4796-91a9-8ee4889cf5cb
- https://aws.amazon.com/ec2/pricing/on-demand/
- https://learn.microsoft.com/en-us/azure/virtual-machines/av2-series
- https://aws.amazon.com/es/ec2/instance-types/
- https://cloud.google.com/compute?hl=es#section-6

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