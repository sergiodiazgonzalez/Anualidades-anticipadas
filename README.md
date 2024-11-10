# Anualidades-anticipadas
Cuando los pagos se realizan al inicio del periodo de pago se llaman anualidades anticipadas.
## Funciones de anualidades anticipadas 
Con el siguiente código, puede usted cargar las funciones de anualidades anticipadas:
```{r}
source("https://raw.githubusercontent.com/sergiodiazgonzalez/Anualidades-anticipadas/refs/heads/main/AnualidadesAnticipadas1.R")
```
A continuación se dan ejemplos del uso de las fórmulas correspondientes
## Valor futuro
$$
VF = A \cdot \frac{(1 + r)^t - 1}{r} \cdot (1 + r)
$$
### Cálculo de valor futuro
Para ilustrar el ejemplo, se tiene el siguiente ejercicio: A=$3,000 t=24 r=5%
Se realizan los cálculos
```{r}
# Creamos objetos con los valores de entrada
Anualidad=3000
NumeroDeAnualidades=24
TasaDeInteres=0.05
# Calulamos el valor futuro
VF=ValorFuturo(A=Anualidad,t=NumeroDeAnualidades,r=TasaDeInteres)
#Imprimimos el resultado:
VF
```
### Cálculo de anualidad con valor futuro
Para ilustrar el ejemplo, se tiene el siguiente ejercicio: VF=$140,181.2965 t=24 r=5%
Se realizan los cálculos
```{r}
# Creamos objetos con los valores de entrada
ValorFuturo=140181.2965
NumeroDeAnualidades=24
TasaDeIntereses=0.05
# Calculamos la anualidad
A=AnualidadValorFuturo(VF=ValorFuturo,t=NumeroDeAnualidades,r=TasaDeIntereses)
#Imprimimos el resultado:
A
```
### Cálculo de Número de Pagos a plazo con valor futuro
Para ilustrar el ejemplo, se tiene el siguiente ejercicio: VF=$140,181.2965 A=$3,000 r=5%
Se realizan los cálculos
```{r}
# Creamos objetos con los valores de entrada
ValorFuturo=140181.2965
Anualidad=3000
TasaDeIntereses=0.05
# Calculamos el número de pagos
t=NumeroDePagosValorFuturo(VF=ValorFuturo,A=Anualidad,r=TasaDeIntereses)
#Imprimimos el resultado:
t
```
### Cálculo de Tasa del periodo con valor futuro
Para ilustrar el ejemplo, se tiene el siguiente ejercicio: VF=$140,181.2965 A=$3,000 t=24
Se realizan los cálculos
```{r}
# Creamos objetos con los valores de entrada
ValorFuturo=140181.2965
Anualidad=3000
NumeroDeAnualidades=24
# Calculamos el número de pago
r=TasaDelPeriodoValorFuturo(VF=ValorFuturo,A=Anualidad,t=NumeroDeAnualidades)
#Imprimimos el resultado:
r
```
## Valor Actual
$$
VA = A \cdot \frac{1 - (1 + r)^{-t}}{r} \cdot (1 + r)
$$
### Cálculo de valor actual
Para ilustrar el ejemplo, se tiene el siguiente ejercicio: A=$3,000 t=24 r=5%
Se realizan los cálculos
```{r}
# Creamos objetos con los valores de entrada
Anualidad=3000
NumeroDeAnualidades=24
TasaDeInteres=0.05
# Calculamos el valor actual
VA=ValorActual(A=Anualidad,t=NumeroDeAnualidades,r=TasaDeInteres)
#Imprimimos el resultado:
VA
```
### Cálculo de anualidad con valor actual
Para ilustrar el ejemplo, se tiene el siguiente ejercicio: VA=$43,465.7217 t=24 r=5%
Se realizan los cálculos
```{r}
# Creamos objetos con los valores de entrada:
ValorActual=43465.7217
NumeroDeAnualidades=24
TasaDeIntereses=0.05
# Calculamos la anualidad
A=AnualidadValorActual(VA=ValorActual,t=NumeroDeAnualidades,r=TasaDeIntereses)
#Imprimimos el resultado:
A
```
### Cálculo de número de Pagos a plazo con valor actual
Para ilustrar el ejemplo, se tiene el siguiente ejercicio: VA=$43,465.7217 A=$3,000 r=5%
Se realizan los cálculos
```{r}
# Creamos objetos con los valores de entrada:
ValorActual=43465.7217
Anualidad=3000
TasaDeIntereses=0.05
# Calculamos el número de pagos
t=NumeroDePagosValorActual(VA=ValorActual,A=Anualidad,r=TasaDeIntereses)
#Imprimimos el resultado:
t
```
### Cálculo de Tasa del periodo con valor actual
Para ilustrar el ejemplo, se tiene el siguiente ejercicio: VA=$43,465.7217 A=$3,000 t=24
Se realizan los cálculos
```{r}
# Creamos objetos con los valores de entradad:
ValorActual=43465.7217
Anualidad=3000
NumeroDeAnualidades=24
# Calculamos la tasa del periodo
r=TasaDelPeriodoValorActual(VA=ValorActual,A=Anualidad,t=NumeroDeAnualidades)
# Imprimimos el resultado
r
```
