# Conjunto de Datos: Predicción de Ventas en Big Mart

## Descripción
Los científicos de datos de **BigMart** recopilaron información de ventas del año 2013 para **1559 productos** en **10 tiendas** ubicadas en diferentes ciudades.  
Además, se definieron ciertos atributos de cada producto y tienda.  

El objetivo es construir un **modelo predictivo** que permita estimar las ventas de cada producto en un punto de venta específico.  
Este modelo ayudará a comprender las propiedades de productos y tiendas que influyen en el incremento de las ventas.  

Nota: El conjunto de datos puede contener valores faltantes debido a fallos técnicos en algunos establecimientos. Será necesario tratarlos adecuadamente.

---

## Diccionario de Datos

### Conjuntos disponibles
- **Train (8523 registros):** contiene variables de entrada y salida (ventas).  
- **Test (5681 registros):** contiene solo variables de entrada; se deben predecir las ventas.

---

### Archivo Train
CSV con información de productos y tiendas, incluyendo el valor de ventas.

**Variables:**
- `Item_Identifier` → ID único del producto  
- `Item_Weight` → Peso del producto  
- `Item_Fat_Content` → Indica si el producto es bajo en grasa  
- `Item_Visibility` → % del área de exhibición asignada al producto en la tienda  
- `Item_Type` → Categoría del producto  
- `Item_MRP` → Precio máximo de venta al público (lista)  
- `Outlet_Identifier` → ID único de la tienda  
- `Outlet_Establishment_Year` → Año de fundación de la tienda  
- `Outlet_Size` → Tamaño de la tienda (área cubierta)  
- `Outlet_Location_Type` → Tipo de ciudad donde se ubica la tienda  
- `Outlet_Type` → Tipo de tienda (supermercado o tienda de abarrotes)  
- `Item_Outlet_Sales` → Ventas del producto en la tienda (variable objetivo a predecir)  

---

### Archivo Test
CSV con combinaciones de productos y tiendas para las cuales se deben pronosticar las ventas.

**Variables:**
- `Item_Identifier` → ID único del producto  
- `Item_Weight` → Peso del producto  
- `Item_Fat_Content` → Bajo en grasa o no  
- `Item_Visibility` → % del área de exhibición asignada  
- `Item_Type` → Categoría del producto  
- `Item_MRP` → Precio máximo de venta al público  
- `Outlet_Identifier` → ID único de la tienda  
- `Outlet_Establishment_Year` → Año de fundación de la tienda  
- `Outlet_Size` → Tamaño de la tienda  
- `Outlet_Location_Type` → Tipo de ciudad  
- `Outlet_Type` → Tipo de tienda (supermercado o abarrotes)  

---

### Archivo de Envío (Submission)
Formato requerido para la predicción final.

**Variables:**
- `Item_Identifier` → ID único del producto  
- `Outlet_Identifier` → ID único de la tienda  
- `Item_Outlet_Sales` → Ventas del producto en la tienda (resultado a predecir)  

---

## Métrica de Evaluación
El desempeño del modelo se evaluará comparando las predicciones de ventas del archivo **test.csv** con los valores reales.  

La métrica utilizada será el **Error Cuadrático Medio (RMSE)**.  
Un menor valor de RMSE indica un mejor ajuste del modelo.
