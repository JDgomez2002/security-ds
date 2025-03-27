# Security Data Science - Threat Hunting Laboratory

## Laboratorio #5: Threat Hunting with Data Science

#### José Daniel Gómez Cabrera 21429

### Objetivos del Laboratorio
- Aplicar conocimientos de threat hunting, data science y dominio experto
- Detectar dominios maliciosos en tráfico de red utilizando técnicas avanzadas

### Descripción del Proyecto

#### Contexto
El laboratorio se enfoca en la identificación de dominios generados por algoritmos (DGA - Domain Generation Algorithms), que son comúnmente utilizados en comunicaciones de malware para evadir soluciones de seguridad tradicionales.

#### Metodología
El proyecto sigue un enfoque de tres etapas para identificar dominios potencialmente maliciosos:

1. **Filtrado y Preprocesamiento**
   - Analizar archivo de tráfico de red capturado por IDS Suricata
   - Filtrar registros DNS
   - Extraer dominios únicos
   - Identificar registros tipo A

2. **Clasificación con Data Science**
   - Utilizar Gemini AI para clasificar dominios como DGA o legítimos
   - Aplicar técnicas de machine learning para detección preliminar

3. **Análisis de Dominio Experto**
   - Verificar dominios contra lista de top 1 millón de TLDs
   - Evaluar fecha de creación de dominios
   - Identificar patrones de generación aleatoria

### Tecnologías Utilizadas
- Python
- Pandas
- Google Gemini AI
- TLD Extraction
- JSON Processing

### Estructura del Repositorio
```
threat-hunting-lab/
│
├── large_eve.json         # Archivo de captura de tráfico de red
├── top-1m.csv             # Lista de top 1 millón de dominios
├── threat_hunting.ipynb   # Notebook principal del análisis
└── README.md              # Documentación del proyecto
```

### Pasos de Ejecución
1. Instalar dependencias
```bash
pip install pandas google-generativeai tldextract
```

2. Configurar API Key de Gemini
3. Ejecutar el notebook Jupyter

### Hallazgos Principales
- Total de registros de red analizados: 746,909
- Registros DNS filtrados: 21,484
- Dominios únicos identificados: 177
- Dominios sospechosos detectados: [Resultado final del análisis]

### Consideraciones de Seguridad
- Los dominios DGA son típicamente:
  - Generados aleatoriamente
  - De corta duración
  - Sin significado semántico
  - Utilizados para comunicación de malware

### Limitaciones
- Dependencia de la precisión del modelo de IA
- Posibilidad de falsos positivos/negativos
- Requiere actualización constante de técnicas de detección

### Contribuciones
Desarrollado como parte del curso CC3067 - Security Data Science
Universidad del Valle de Guatemala
Semestre I - 2025

### Licencia
Proyecto académico - Uso educativo