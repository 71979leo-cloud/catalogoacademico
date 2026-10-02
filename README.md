# Catalogo de Recursos Academicos

## Descripcion

Catalogo de Recursos Academicos es un proyecto inicial para organizar recursos de estudio en un catalogo estructurado.

## Objetivo

Establecer una base sencilla para registrar y consultar recursos academicos clasificados por tipo, tema, nivel y autor o fuente.

## Estructura general

```text
app/                 Codigo de la aplicacion
	configuracion.py   Espacio reservado para configuracion
	main.py            Punto de entrada inicial
data/                Datos del catalogo
	recursos.json      Registros de ejemplo
docs/                Documentacion de alcance y criterios
test/                Pruebas del proyecto
CHANGELOG.md         Historial de cambios
requirements.txt     Dependencias de Python
```

## Tecnologias y dependencias

- Python 3.10 o posterior
- JSON para almacenar los registros iniciales
- Dependencias Python declaradas en `requirements.txt`

La salida inicial solo usa la biblioteca estandar de Python. El archivo de dependencias conserva el entorno registrado para el proyecto y puede instalarse con pip.

## Preparar el entorno

Desde la carpeta del proyecto, crea y activa un entorno virtual en PowerShell:

```powershell
py -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

En macOS o Linux, usa estos comandos para crear y activar el entorno:

```sh
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

Ejecuta el punto de entrada inicial con:

```sh
python app/main.py
```

## Próximas mejoras

- Permitir agregar, editar y eliminar recursos desde una interfaz.
- Incorporar búsqueda y filtros por tipo, tema, nivel y autor o fuente.
- Validar los datos antes de guardar cambios en el catálogo.
