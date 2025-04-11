# Examen ED 
### Nuria Alba Ortega


# Errores

## 1.- Replace this use of System.out by a logger

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

## 2.- Use the built-in formatting to construct this argument

He cambiado esto:

```
logger.info("...")
```
Por esto:

```
logger.log(Level.SEVERE,() -> "..." + ...);
```

## 3.- 






