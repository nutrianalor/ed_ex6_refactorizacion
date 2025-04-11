# Examen ED 
### Nuria Alba Ortega


# Errores

> ## 1.- Replace this use of System.out by a logger

Para este corregir este error escribimos lo siguiente afuera de la clase:

```
import java.util.logging.Logger;
```

Después adentro de la clase:

```
Logger logger = Logger.getLogger(getClass().getName());
```
Y por último sustituimos todos los System.out por logger.info:

```
logger.info("...")
```

>## 2.- Use the built-in formatting to construct this argument

He cambiado esto:

```
logger.info("...")
```
Por esto:

```
logger.log(Level.SEVERE,() -> "..." + ...);
```

>## 3.- Remove this expression which always evaluates to "true"

Lo único que he cambiado en este error para hacerlo desaparecer ah sido quitar `"!="` y en su lugar poner `"=="`.
```
if (notasRA == null)
```

>## 4.- Remove this unused label.

He eliminado `label{}` al completo.

>## 5.- Merge this if statement with the enclosing one

He fusionado una condicional que estaba dentro de otra:

```
if (notasRA == null && notasRA.size() > 0)
```







