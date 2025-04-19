# Venta de Productos con Analisis de datos en Power Bi
<p>
  
 #### Descripción de la temática de los datos
  </p>
  <p>
Este conjunto de datos sobre Ventas de Productos se presenta como una compilación completa de información que abarca los productos en venta, así como el inicio y final de los convenios establecidos entre la empresa y los clientes, incluyendo detalles de las respectivas facturas y pagos.
</p>

  #### Hipotesis

Al se estudiar el cliente se puede saber cual los produto a investir.

<b>Descriptivo:</b> Comprender y describir los patrones actuales y pasados de la venta de Productos
<p>- Calcular estadísticas descriptivas como promedios, medianas, desviaciones estándar, etc., para variables relevantes como ventas, pagos y descuentos.</p>
<p>- Crear gráficos para visualizar tendencias y distribuciones.</p>
<p> - Analizar la composición de ventas por delegación, empleado, cliente, etc.</p>
<p><b>Diagnóstico:</b> Identificar las razones detrás de ciertos patrones y tendencias observadas.</p>
<p>- Realizar análisis de correlación para entender la relación entre variables como ventas y descuentos, pagos y facturas, etc.</p>
<p>- Identificar outliers o valores atípicos que podrían requerir una mayor investigación.</p>
<p> - Utilizar visualizaciones avanzadas para identificar tendencias temporales o   patrones    específicos.</p>
<p><b>Predictivo:</b>Prever futuros patrones y comportamientos en función de datos históricos.</p>
<p>- Implementar modelos de regresión para prever ventas futuras o montos de pagos.</p>
<p>- Utilizar algoritmos de clasificación para prever la probabilidad de que un cliente acepte un convenio.</p>
<p>- Dividir el conjunto de datos en conjuntos de entrenamiento y prueba para evaluar la precisión del modelo.</p>
<p><b>Prescriptivo:</b> Sugerir acciones y estrategias para mejorar el rendimiento y la eficiencia basándose en los resultados predictivos. </p>
<p>- Desarrollar recomendaciones para mejorar la eficiencia de las ventas basadas en patrones identificados.</p>
<p>- Sugerir estrategias de descuentos o convenios para maximizar las ventas y retener clientes.</p>
<p>- Sugerir estrategias de descuentos o convenios para maximizar las ventas y retener clientes.</p>
<p>- Proporcionar insights sobre el rendimiento de los empleados y delegaciones para optimizar la asignación de recursos.</p>
<p>Para garantizamos que la descripción de la temática cumpla con los principios de la metodología SMART:</p>
<p><b>Específico (Specific):</b> El conjunto de datos se centra específicamente en proporcionar información detallada sobre las transacciones de venta, acuerdos con clientes y las transacciones financieras asociadas.</p>
<p><b>Medible (Measurable):</b> Se incluyen datos cuantificables como ventas, pagos, descuentos, inicio y final de convenios, permitiendo la aplicación de estadísticas descriptivas y análisis correlativos para medir y entender las tendencias del negocio.</p>
<p> <b>Alcanzable (Achievable):</b> La información recopilada es realista y alcanzable, reflejando de manera precisa la actividad comercial y financiera de la empresa en relación con sus productos.</p>
<p><b>Relevante (Relevant):</b> La temática es relevante para la toma de decisiones estratégicas, ya que proporciona insights sobre la efectividad de las ventas, la gestión de clientes y la eficiencia financiera.</p>
<p>El conjunto de datos abarca un periodo temporal específico, permitiendo análisis históricos y facilitando la aplicación de modelos predictivos para comprender y prever patrones futuros.</p>

#### Alcance, Usuario final y nivel de aplicación
<p>El análisis de estos datos permite calcular estadísticas y crear visualizaciones para comprender los patrones de ventas actuales y pasados, así como identificar oportunidades y áreas a mejorar. Tambien puede servir como base para la toma de decisiones a largo plazo, como la planificación de estrategias de ventas, la segmentación de clientes, el desarrollo de políticas de precios, y la identificación de áreas de crecimiento y expansión del negocio.</p>

#### Dataset
<p>A continuación, se Adjunta el Dataset utilizado para el trabajo:
https://docs.google.com/spreadsheets/d/1cAKkUuACrkbIBD5iTlMMpK9x7IZ5p2Ts/edit?usp=sharing&ouid=112704212058160105170&rtpof=true&sd=true</p>


#### Diagrama entidad-relación

![image](https://github.com/lagmagalhaes/Projeto-Analise-de-Dados/assets/166879716/ff3484e8-254f-4d0e-bf62-e9586abea533)

#### Listado de tablas
<p><b>Clientes:</b></p>
<p>La tabla “Clientes” almacena información detallada sobre los clientes, incluyendo sus datos personales, información de contacto y cualquier detalle relevante que facilite una relación comercial efectiva. Esta tabla sirve como base para establecer conexiones con otras tablas, como “Facturas”, donde la “id_cliente fk” vincula cada factura a un cliente específico.</p>
<p>PK: ID_CLIENTE</p>
<p><b>Convenio:</b></p>
<p>El "Convenio" registra acuerdos o contratos especiales con clientes, brindando un marco para la gestión de descuentos, términos de pago u otras condiciones especiales que puedan afectar las transacciones de venta.</p>
<p>PK : ID_Convenio</p>
<p>FK : ID_Cliente</p>
<p>FK : ID_Delegación</p>
<p><b>Delegación:</b></p>
<p>La tabla "Delegación" se utiliza para organizar y gestionar las distintas delegaciones o sucursales de la empresa. Esto es crucial para negocios con presencia geográfica diversa, ya que permite un seguimiento preciso de las ventas en cada ubicación.</p>
<p>PK: ID_Delegación</p>

<p><b>Empleados:</b></p>
<p>Los "Empleados" son parte integral del proceso de venta, y la tabla correspondiente almacena información sobre el personal de ventas.</p>
<p>PK: ID_Empleado</p>

<p><b>Facturas:</b></p>
<p>Las transacciones comerciales se registran en la tabla "Facturas", donde cada factura y se conecta a clientes, empleados y produtos.</p>
<p>PK:ID_Factura</p>
<p>FK: Id_Cliente</p>
<p>FK:ID_Empleado</p>
<p>FK: ID_Venta</p>
<p>FK: Producto</p>

<p><b>Pago:</b></p>
<p>La tabla "Pago" rastrea los pagos asociados a cada factura, proporcionando una visión completa del ciclo financiero de la venta.</p>
<p>PK: ID_Pago</p>
<p>FK: ID_Factura</p>
<p>FK: ID_Cliente</p>

<p><b>Productos:</b></p>
<p>La tabla "Productos" detalla la gama de productos disponibles para la venta, incluyendo información sobre inventario, precios y otros detalles esenciales. Por último, la tabla "Venta" actúa como un registro central para todas las transacciones de venta, conectando productos, empleados y clientes en un único punto de referencia.</p>
<p>PK: ID_Produtos</p>

<p><b>Venta:</b></p>
<p>La tabla "Venta" registra información detallada sobre las transacciones de venta realizadas por la empresa.</p>
<p>PK: ID_Venta</p>

#### Listado de columnas de tablas
<p>La venta de productos es un proceso crucial en cualquier negocio, y la gestión eficiente de la información relacionada es esencial para el éxito comercial. En este contexto, las tablas fundamentales que integran el sistema de ventas incluyen "Clientes", "Convenio", "Delegación", "Empleados", "Facturas", "Pago", "Productos" y "Venta". Cada una desempeña un papel específico en el seguimiento y la optimización de las operaciones de venta.
A la continuación , se hara mención de las columnas que posee cada tabla junto com su tipo de campo y claves:</p> 

![image](https://github.com/lagmagalhaes/Projeto-Analise-de-Dados/assets/166879716/8aca9305-3d94-47cd-af27-bc7838c7d364)


![image](https://github.com/lagmagalhaes/Projeto-Analise-de-Dados/assets/166879716/56562acc-ee7d-4b0a-bfac-1f0bdf25571a)


<p>En conjunto, estas tablas forman un sistema integral que facilita la gestión eficiente de la venta de productos, desde la interacción con clientes hasta el seguimiento detallado de cada transacción y pago, contribuyendo al crecimiento y la eficacia del negocio.</p> 

#### Transformación de Datos
<p>A continuación se detallan todas las modificaciones realizadas en las diferentes tablas del proyecto final.</p> 
<p><b>Tabla Clientes:</b></p> 
<p>•	Detectar tipo de datos.</p>
<p>•	La columna ID_Cliente se cambio del tipo de número decimal a tipo texto.</p>
<p>•	La columna Teléfono se cambio del tipo de datos de número entero a tipo texto porque cambiar el tipo de datos a texto evitará que se pierdan los ceros iniciales y acepta caracteres.</p>
<p>•	Quitar filas en blanco.</p>

<p><b>Tabla Convenio:</b></p> 
<p>•	Detectar tipo de datos.</p>
<p>•	La columna ID_Convenio se cambio del tipo de número decimal a tipo texto.</p>
<p>•	La columna ID_Cliente se cambio del tipo de número decimal a tipo texto.</p>
<p>•	La columna ID_Delegación se cambio del tipo de número decimal a tipo texto.</p>
<p>•	Quitar filas en blanco.</p>
<p>•	Se redondeó a 2 casas decimales la columna CosteConvenio.</p>

<p><b>Tabla Delegación:</b></p> 
<p>•	Detectar tipo de datos.</p>
<p>•	La columna ID_Delegación se cambio del tipo de número decimal a tipo texto.</p>
<p><b>Tabla Empleados:</b></p> 
<p>•	Detectar tipo de datos.</p>
<p>•	La columna ID_Empleados se cambio del tipo de número decimal a tipo texto.</p>

<p><b>Tabla Facturas:</b></p> 
<p><•	Detectar tipo de datos.</p>
<p>•	La columna ID_Facturas se cambio del tipo de número decimal a tipo texto.</p>
<p>•	Quitar filas en blanco.</p>
<p>•	Se redondeó a 2 casas decimales la columna ImporteSinImpuesto. </p>
<p>•	Se redondeó a 2 casas decimales la columna Impuesto.</p>

<p><b>Tabla Pago:</b></p> 
<p>•	Detectar tipo de datos.</p>
<p>•	La columna ID_Pago se cambio del tipo de número decimal a tipo texto.</p>
<p>•	La columna ID_Factura se cambio del tipo de número decimal a tipo texto.</p>
<p>•	La columna ID_Cliente se cambio del tipo de número decimal a tipo texto.</p>
<p>•	Quitar filas en blanco.</p>
<p>•	Se redondeó a 2 casas decimales la columna ImportePagado.</p> 

<p><b>Tabla Productos:</b></p> 
<p>•	Detectar tipo de datos.</p>
<p>•	La columna ID_Poductos se cambio del tipo de número decimal a tipo texto.</p>
<p>•	Quitar filas en blanco.</p>
<p>•	Se redondeó a 2 casas decimales la columna Precio Unitario.</p>
<p><b>Tabla Venta:</b></p> 
<p>•	Detectar tipo de datos.</p></p>
<p>•	La columna ID_Venta se cambio del tipo de número decimal a tipo texto.

<p><b>Medidas calculadas</b></p>

![image](https://github.com/user-attachments/assets/edfa563a-7992-45ce-abfe-1ea01570b613)


<p><b>Modelo relacional de Power BI</b></p>

![image](https://github.com/lagmagalhaes/Projeto-Analise-de-Dados/assets/166879716/1d73edd7-d058-4a96-a226-eeacc0876c3a)
<p><b>Futuras Líneas</b></p>
<p>A futuro se recomenda a generar un dashboard que haga la comparación de la Facturación por Marca y outro dashboard con los datos de cual la Delegación que más vende con un gráfico de Mapa.</p>
<p><b>Dashboard y Descripción</b></p>
<p><b>Dashboard Portada</b></p>
<p>En esta solapa se presenta el Proyecto y los dashboard de Cliente, Facturación y Productos.<p>

  
![image](https://github.com/user-attachments/assets/94433f67-40fd-4bb5-b0c6-a8c2611d465b)

  
![image](https://github.com/user-attachments/assets/622b3f46-3804-4d37-b66a-bc3efc2f827c)


![image](https://github.com/user-attachments/assets/97e3d20f-61ba-4d53-9703-d1ecfce33df5)


![image](https://github.com/user-attachments/assets/91eba263-05e2-4b9f-a76b-1110bf0461cc)


![image](https://github.com/user-attachments/assets/7d16a7e4-3484-4ff8-b881-4ec735296ba2)













