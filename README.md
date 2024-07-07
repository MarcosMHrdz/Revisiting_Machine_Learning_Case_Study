![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Lab | Revisión del estudio de caso de aprendizaje automático

- En este laboratorio, utilizarás el archivo `learningSet.csv` que ya clonaste en las actividades de hoy.

### Instrucciones

Complete los siguientes pasos en las columnas categóricas del conjunto de datos:

- Verificar valores nulos en todas las columnas
- Excluya las siguientes variables consultando las definiciones. Cree una nueva lista vacía llamada `drop_list`. Anexaremos esta lista y luego eliminaremos todas las columnas de esta lista:
    - `OSOURCE` - no se proporcionan definiciones de símbolos, demasiadas categorías
    - CÓDIGO POSTAL - ya estamos incluyendo el estado
- Identificar columnas en las que faltan más del 85 % de valores
- Eliminar esas columnas del marco de datos
- Reducir la cantidad de categorías en la columna "GÉNERO". La columna solo debe tener "M" para hombres, "F" para mujeres y "otro" para el resto.
    - Tenga en cuenta que hay algunos valores nulos en la columna. Primero reemplazaremos esos valores nulos con el código que se muestra a continuación:

    ``pitón
    imprimir(categorical['GÉNERO'].value_counts())
    categórico['GÉNERO'] = categórico['GÉNERO'].fillna('F')
    ```
