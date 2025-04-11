# Examen ED 
### Nuria Alba Ortega


# Errores

## 1.- Move this file to a named package.

Es una mala práctica colocar todas las clases directamente en el directorio fuente de un proyecto sin una estructura de paquete.

He creado un paquete con nombre y he movido el .java ahí.

## 2.- Replace this use of System.out by a logger.

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

