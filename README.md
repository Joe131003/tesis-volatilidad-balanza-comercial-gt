# Volatilidad de los precios internacionales y saldo comercial de Guatemala (2010–2024)

Código y datos de replicación de la tesis de licenciatura en Economía:

> Estrada Morales, J. A. (2026). *Volatilidad de los precios internacionales del café, azúcar, banano, cardamomo y petróleo y su asociación con el saldo de la balanza comercial de Guatemala (2010–2024): un análisis mediante modelos GARCH y ARDL*. Universidad Rafael Landívar.

Con estos archivos se reproducen todas las tablas y figuras del capítulo de resultados.

## Archivos

| Archivo | Qué hace |
| --- | --- |
| `Base_datos_tesis.xlsx` | Base de datos mensual 2010–2024. La hoja `BASE_CORREGIDA` es la que usa el código. |
| `codigo_tesis_v1.ipynb` | Análisis principal: volatilidad (GARCH, GJR-GARCH y EGARCH), pruebas de integración, ARDL con prueba de límites, diagnósticos, bootstrap, robustez y Toda–Yamamoto. |
| `nardl_complementario.ipynb` | Análisis complementario NARDL de alzas y bajas de precios. |
| `figuras_tesis.ipynb` | Figura 2 y Figuras 4 a 9 de la tesis. |
| `requirements.txt` | Librerías de Python necesarias. |

## Cómo reproducir los resultados

1. Instalar Python 3.11 o superior y las librerías: `pip install -r requirements.txt`
2. Dejar los cuatro archivos (la base y los tres notebooks) en la misma carpeta.
3. Correr en este orden: `codigo_tesis_v1`, `nardl_complementario` y `figuras_tesis`.

Cada notebook crea su propia carpeta de resultados. El análisis principal tarda unos tres minutos. Las simulaciones usan una semilla fija, así que los resultados son idénticos en cada corrida.

## Fuentes de los datos

| Variable | Fuente |
| --- | --- |
| Exportaciones e importaciones de bienes | FMI, Direction of Trade Statistics, ajustado a los totales anuales del Banco de Guatemala |
| Café, azúcar, banano y petróleo WTI | Banco Mundial, Pink Sheet |
| Cardamomo (valor unitario de exportación) | UN Comtrade |
| Tipo de cambio nominal y remesas | Banco de Guatemala |
| ITCER | SECMCA |

Los datos pertenecen a sus fuentes originales. El código tiene licencia MIT.
