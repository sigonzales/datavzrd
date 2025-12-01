# Reporte interactivo de variantes CYP en pacientes con esquizofrenia resistente al tratamiento, tratados con clozapina  
**Bioinformática – Data Visualization**  
Proyecto realizado con **DataVzrd (2025)**

Este repositorio contiene un reporte interactivo generado con **DataVzrd**, donde se visualizan datos clínicos, farmacogenómicos y genéticos de una cohorte de 47 pacientes tratados con clozapina en Uruguay.  
Incluye análisis de variantes individuales (SNPs), haplotipos y perfiles metabolizadores de los genes **CYP1A2, CYP2C19, CYP2D6 y CYP3A4**.
---

## Contenido del repositorio

### **1. Archivo de configuración**
- `clozapina.yaml`  
  Contiene toda la configuración de DataVzrd:  
  - vistas (`views`)  
  - columnas personalizadas  
  - heatmaps  
  - enlaces externos (PharmVar, SNPs)  
  - gráficos Vega-Lite  
  - uniones entre tablas  

### **2. Datos**
Ubicados en la carpeta `data/`:

- `tabla_clozapina_agosto2025.csv`  
  Datos clínicos, genéticos y metabolizadores CYP.

- `samples47_comparaciones_haplotipos.csv`  
  Haplotipos, frecuencias y comparaciones con PharmVar.

- `samples47_comparaciones_snps.csv`  
  SNPs anotados por ANNOVAR, frecuencias globales y comparaciones con 1000G y gnomAD 4.1.

### **3. Reporte generado**
- Carpeta `reporte_clozapina/`  
  Contiene la salida HTML completa generada por DataVzrd.

## Reproducir el reporte

### **1. Instalar DataVzrd**
```bash
pip install datavzrd
```

### **2. Generar el reporte**
Ejecutar desde la carpeta raíz:

```bash
datavzrd clozapina.yaml --output reporte_clozapina --overwrite-output
```

## Autora
Sofía Gonzales Magallanes
Unidad de Bioinformática – Institut Pasteur de Montevideo
GitHub: @sigonzales
