# Laboratorio #6 - Análisis de tráfico de red

### José Daniel Gómez Cabrea 21429

Este laboratorio forma parte del curso CC3094 - Security Data Science de la Universidad del Valle de Guatemala. El objetivo principal es aplicar conocimientos sobre redes de computadoras en el análisis estadístico de tráfico de red para detectar anomalías en el comportamiento de la red.

## Objetivos
- Aplicar los conocimientos sobre redes de computadoras en el análisis estadístico de tráfico de red
- Detectar anomalías en el comportamiento de la red mediante análisis de datos
- Familiarizarse con herramientas de captura y análisis de paquetes de red

## Requisitos Previos
- Python 3.8 o superior
- Jupyter Notebook
- Conexión a internet para la instalación de paquetes
- Archivo `analisis_paquetes.pcap` (disponible en CANVAS)

## Guía de Instalación

### 1. Entorno Virtual (Recomendado)
Primero, crea y activa un entorno virtual para mantener las dependencias aisladas:

```bash
# Crear entorno virtual
python -m venv venv

# Activar entorno virtual
# En Windows:
venv\Scripts\activate
# En macOS/Linux:
source venv/bin/activate
```

### 2. Instalación de Dependencias
Instala las bibliotecas necesarias para el laboratorio:

```bash
# Instalar Jupyter Notebook
pip install notebook

# Instalar Scapy
pip install scapy

# Instalar pandas para análisis de datos
pip install pandas

# Instalar matplotlib y seaborn para visualizaciones
pip install matplotlib seaborn

# Instalación de dependencias adicionales
pip install numpy ipywidgets
```

### 3. Instalar Wireshark (Opcional, pero recomendado)
Aunque no es estrictamente necesario para este laboratorio, Wireshark puede ser útil para inspeccionar visualmente los archivos PCAP.

- **Windows/macOS**: Descarga e instala desde [wireshark.org](https://www.wireshark.org/download.html)
- **Linux**:
  ```bash
  sudo apt-get install wireshark    # Para distribuciones basadas en Debian/Ubuntu
  sudo dnf install wireshark        # Para distribuciones basadas en Fedora
  ```

## Configuración del Entorno

### 1. Descargar Archivo PCAP
Asegúrate de descargar el archivo `analisis_paquetes.pcap` desde CANVAS y guárdalo en la carpeta del proyecto.

### 2. Iniciar Jupyter Notebook
```bash
jupyter notebook
```
