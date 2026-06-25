# -Regresan-los-usuarios-de-RappiPlus-

Realicé un análisis para saber si los clientes del servicio de Rappiplus regresan a utilizar el servicio después de probarlo, ver en que parte del funnel de conversión hay mayor drop de usuarios y los ingresos o pérdidas generados en ventas. 
Proceso: 
Lo primero fue realizar la limpieza de 3 datasets con python para que los datos fueran confiables, después cálcule los costos, gastos de mkt y los ingresos. El verdadero reto fue dejar los datos en condiciones optimas ya que había múltiples datos faltantes en distintas categorías y outliers extremos en cantidades de ventas.
Posteriormente con SQL revise el embudo de conversión para ver en que parte del proceso se pierden más clientes y un análisis de cohortes para ver si los clientes que compran regresan en el futuro.
También realicé una prueba estadística Z en un experimento A/B para saber si el aumento en los clientes se debía al azar o ralmente a las mejoras en la página.
Por último con los 3 datasets limpios creé un dashboard en PowerBi para un análisis más detallado sobre las ventas.
Resultado: Lo que cambió: números o lecciones
Los hallazgos más críticos fueron que del checkout al pago es el proceso donde se tienen más pérdidas y que uno de los productos generaba pérdidas ya que sus costos eran más altos que el revenue. La lección de esto es que hay que hacer una revisión de si el metodo de pago es muy complicado o tiene algún error en la plataforma para disminuir el drop, y por otra parte se tiene que implementar un sistema de control al momento de fijar precios de venta en los productos para evitar ventas que generen pérdidas.
