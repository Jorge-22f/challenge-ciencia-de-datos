# challenge-ciencia-de-datos

# **Análisis de Rentabilidad y Ventas por Tienda**  

Este proyecto analiza datos de ventas de diferentes tiendas para identificar patrones y recomendar estrategias basadas en rentabilidad, satisfacción del cliente y distribución geográfica de ventas.

## **Tabla contenido**

* Instalación y Configuración
* Dependencias Utilizadas
* Cómo Ejecutar el Proyecto
1. Carga y visualización de datos
2. ingresos totales
3. Categorías Más Vendidas
4. Calificación Promedio de Clientes
5. Productos mas y menos vendidos
6. Costo Promedio de Envío
7. Rentabilidad
8. Desempeño empleados
9. conclucion
10. Analisis del desempeño geografico
* Posibles Problemas y Soluciones

## **Instalación y Configuración**  

Este análisis se ejecuta en **Google Colab**, por lo que no es necesario instalar nada localmente. Para correrlo correctamente, sigue estos pasos:  

1. **Abre Google Colab**.  
2. **Sube los archivos de datos** (`AluraStoreLatamipynb`).  
3. **Ejecuta el código en orden**, asegurando que todas las dependencias estén correctamente instaladas.
4. **Código base:** Ya está listo para extraer y organizar los datos correctamente, se recomienda no modificarlo. 

Los datos de cada tienda están disponibles en archivos CSV y se cargarán utilizando el código base ya proporcionado. El código extrae información de las cuatro tiendas y organiza los datos en DataFrames utilizando la biblioteca Pandas.

Si deseas correr este proyecto localmente, asegúrate de instalar las siguientes dependencias usando `pip`:  

```bash
pip install pandas matplotlib seaborn folium
```

## **Dependencias Utilizadas**  

Durante el análisis se emplearon las siguientes bibliotecas:  

- `pandas` → Para manipulación y análisis de datos.  
- `matplotlib` → Para generar gráficos de barras y dispersión.  
- `seaborn` → Para visualizaciones avanzadas como gráficos de violín.  
- `folium` → Para mapas interactivos y mapas de calor.  

## **Cómo Ejecutar el Proyecto**  

Ejecutar este análisis es sencillo. Sigue este flujo para evitar errores:  

1. **Carga y visualización de datos**:  
   - Ejecuta la primera celda que importa y carga los archivos (`tienda_1 ,tienda_2, tienda_3 y tienda_4`).

    - Los datos se cargaran a las variables (`tienda ,tienda2, tienda3 y tienda4`)    
    
2. **Análisis de Facturación**:  
   - Ejecuta el bloque de código donde se calculan ingresos totales por tienda.  
   - Verifica que los valores están correctos antes de continuar.
   - Al final del bloque se debe renderizar el grafico comparacion facturacion por tienda.

3. **Comparaciones de Ventas por categoría**:  
   - Ejecuta los bloques de cálculo de ventas por categoría y productos más vendidos.  
   - Cada linea mostrara las categorias de los productos mas populares en la tienda junto con el numero de productos vendidos de esa categoria.

4. **Calificación promedio de la tienda**:
   - Ejecuta el bloque de código donde se calcula la calificacion promedio de la tienda.
   - Verifica que los valores están correctos antes de continuar.
   - Al final del bloque se debe renderizar el grafico comparacion de las calificaciones por tienda.
   - Si desea ver la distribucion de las calificaciones por cada tienda al final del bloque encontrara un script para renderizar un grafico de violin si desea ver otra tienda solo cambie la variable de la tienda:
   (`tienda ,tienda2, tienda3 y tienda4`).
   En la linea:
   df = pd.DataFrame(data_tienda3).

5. **Productos más y menos vendidos**:
   - Ejecuta el bloque de código donde se calcula los productos mas y menos vendidos de cada tienda.
   - Verifica que los valores están correctos antes de continuar.
   - Cada linea mostrara en una lista los productos mas vendidos junto con los productos menos vendidos de cada tienda y la cantidad vendida de cada uno.

6. **Envío promedio por tienda**:
   - Ejecuta el bloque de código donde se calcula el promedio del costo del envio de cada tienda.
   - Verifica que los valores están correctos antes de continuar.
   - Cada linea mostrara el costo promedio del envio.
   - Al final del bloque se debe renderizar el grafico comparacion de costo promedio del envio por tienda.

7. **Rentabilidad promedio ingresos totales vs costo envio**:
   - Ejecuta cada bloque de código para calcular la rentabilidad de cada tienda.
   - Verifica que los valores están correctos antes de continuar.
   - Cada linea mostrara la rentabilidad de cada tienda.
   - Al final del bloque se debe renderizar el grafico comparativo que mostrara la rentabilidad de cada tienda.

8. **Analisis del desempeño de empleados**:
   - Ejecuta el bloque de código donde se calcula el analisis del desempeño de empleados de cada tienda.
   - Verifica que los valores están correctos antes de continuar.
   - Cada linea mostrara en una lista donde se podra visualizar los empleados de cada tienda, el numero de ventas y el total del valor de las ventas.

9. **Análisis Comparativo de Rendimiento de Tiendas**:
    En esta seccion se mostrara el analisis donde se analizan los datos recopilados a lo largo del proyecto se identifican patrones y se recomendan estrategias basadas en cada punto.

10. **Analisis del desempeño geografico** *(Punto opcional)*:  
   - Ejecuta el código de `folium` para generar el mapa interactivo.  
   - Ajusta el nivel de zoom en `folium.Map()` si quieres mejorar la visualización.
   - Si desea ver la distribucion de las ventas de cada tienda encontrara un script para renderizar un grafico de dispercion. si desea ver otra tienda solo cambie la variable de la tienda:
   (`tienda ,tienda2, tienda3 y tienda4`).
   En la linea:
   grafico_geografico_ventas(tienda)
   - Si desea ver la distribucion de las ventas de cada tienda encontrara un script para renderizar un Mapa Interactivo. si desea ver otra tienda solo cambie la variable de la tienda:
   (`tienda ,tienda2, tienda3 y tienda4`).
   En la linea:
   df = pd.DataFrame(tienda4) 

## **Posibles Problemas y Soluciones**  

🚨 **Error: No se encuentra el archivo de datos**  
📌 **Solución**: Ejecuta la primera celda que importa y carga los archivos  

🚨 **Error: Los gráficos no se generan correctamente**  
📌 **Solución**: Asegúrate de ejecutar los bloques de análisis **en orden**, primero cargando datos, luego haciendo cálculos y finalmente generando visualizaciones.
