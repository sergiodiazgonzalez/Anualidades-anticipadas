# Anualidades-anticipadas
Cuando los pagos se realizan al inicio del periodo de pago se llaman anualidades anticipadas.
## Funciones de anualidades anticipadas 
Con el siguiente código, puede usted cargar las funciones de anualidades anticipadas:
```{r}
source("https://raw.githubusercontent.com/sergiodiazgonzalez/Anualidades-anticipadas/refs/heads/main/AnualidadesAnticipadas.R")
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
