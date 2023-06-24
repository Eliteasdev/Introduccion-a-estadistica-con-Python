1. Los datos siguientes muestran los pesos de 50 estudiantes que se registraron con aproximación de una libra.
```python
datos = [159, 136, 180, 129, 162, 150, 129, 146, 128, 178, 144, 167, 132, 172, 156, 178, 129, 142, 146, 159, 131, 135, 168, 152, 163, 145, 173, 147, 137, 143, 142, 133, 152, 166, 146, 131, 131, 160, 162, 146, 151, 179, 146, 142, 172, 175, 166, 137, 162, 159]
```
2. Se obtuvo la medición de una serie de tornillos que se tienen que embarcar, pero se quiere sacar una estadística escriptiva de las mediciones.
```python
datos2 = [1.34, 1.2, 1.41, 1.52, 1.49, 1.3, 1.24, 1.29, 1.53, 1.55, 1.37, 1.56, 1.56, 1.39, 1.39, 1.51, 1.59, 1.54, 1.29, 1.44, 1.5, 1.22, 1.32, 1.42, 1.42, 1.6, 1.58, 1.31, 1.45, 1.29, 1.51, 1.4, 1.29, 1.57, 1.24, 1.44, 1.28, 1.52, 1.49, 1.41, 1.32, 1.31, 1.23, 1.25, 1.57, 1.53, 1.35, 1.57, 1.50, 1.49]
```
De los datos de arriba encontrar la siguiente información:
* El valor más grande
```python
print(n.max(datos))
```
* El valor más pequeño
```python
print(np.min(datos))
```
* Obtuvieron 125(datos 1), 1.25(datos 2) o mas
```python
get_125 = np.where(datos>=125,1,0).sum()
get_1_25 = np.where(datos2>=1.25,1,0).sum()
```
* Obtuvieron 138(datos 1), 1.32(datos 2) o menos
```python
get_138 = np.where(datos<=138,1,0).sum()
get_1_32 = np.where(datos2<=1.32,1,0).sum()
```
* Porcentaje de valores (129<=x>=146, dato1), (1.39< x >=141, dato2)

```python
porcentaje = np.where((datos>=129) && (datos <=146),1,0).sum() / datos.lenght
print(porcentaje*100, "%")
porcentaje2 = np.where((datos2>=1.39) && (datos2 <=1.41),1,0).sum() / datos.lenght
print(porcentaje2*100, "%")
```
* Frecuencias absolutas simples
```python
fig, ax = plt.subplots()
variables, repetidas =np.unique(datos, return_counts=True)
```
* Frecuencias absolutas acumuladas
* Frecuencias relativas simples
* Frecuencias relativas acumuladas
* Media aritmética valores agrupados
* Media aritmética de valores no agrupados
* Media Geométrica
* Media Armónica H
* Mediana
* Moda
* Múltiples Modas (si las hay)
* Cuartiles
* Deciles
* Percentiles
* Realizar el histograma con Matplotlib


```python
```