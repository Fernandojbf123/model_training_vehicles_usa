# Predicción de precio de vehículos usados

Este proyecto desarrolla un flujo de análisis y modelado para estimar el precio de venta de autos usados.

## Descripción

El trabajo incluye:

- EDA (Análisis Exploratorio de Datos) del dataset de vehículos.
- Limpieza y preparación de datos.
- Entrenamiento y comparación de varios modelos de Machine Learning.
- Selección del mejor modelo para predecir precios.

## Caso de uso

Un revendedor quiere construir un sistema que, cuando una persona llegue a ofrecer su auto, permita estimar rápidamente un precio de compra/venta sugerido usando un modelo entrenado.

Con este enfoque, el negocio puede:

- Tener una referencia de precio basada en datos.
- Reducir la variabilidad entre tasaciones.
- Tomar decisiones de compra con mayor confianza.

## Estructura del proyecto

- `main.ipynb`: notebook principal con EDA y entrenamiento de modelos.
- `datasets/car_data.csv`: dataset base.
- `pyproject.toml`: configuración del proyecto y dependencias.

## Instalación con UV

Este proyecto utiliza [UV](https://docs.astral.sh/uv/) como gestor de paquetes y entorno.

### Requisitos previos

- Python 3.10+ (recomendado).
- Git (opcional, para clonar el repositorio).

### Linux

1. Instalar UV:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

2. Recargar la terminal (o abrir una nueva) y verificar instalación:

```bash
uv --version
```

3. Desde la raíz del proyecto, instalar dependencias:

```bash
uv sync
```

4. Ejecutar Jupyter Notebook con el entorno del proyecto:

```bash
uv run jupyter notebook
```

### Windows

1. Instalar UV con PowerShell:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

2. Cerrar y abrir la terminal, luego verificar:

```powershell
uv --version
```

3. Desde la raíz del proyecto, instalar dependencias:

```powershell
uv sync
```

4. Ejecutar Jupyter Notebook con el entorno del proyecto:

```powershell
uv run jupyter notebook
```

## Uso general

1. Abrir `main.ipynb`.
2. Ejecutar las celdas en orden para:
	- explorar datos,
	- entrenar modelos,
	- evaluar métricas,
	- generar predicciones de precio.

## Resultado esperado

Obtener un modelo capaz de estimar el precio de un vehículo usado a partir de sus características, para apoyar la negociación y compra por parte del revendedor.
