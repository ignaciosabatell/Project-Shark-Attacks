# 🦈 Shark Encounters Analysis

## 📄 Descripción
Este proyecto analiza un dataset global de encuentros con tiburones para identificar patrones de riesgo, oportunidades de seguros marítimos y actividades acuáticas más frecuentes.  

Se han realizado las siguientes tareas:  
- Limpieza y normalización de columnas (`species`, `age`, `fatal_y/n`, etc.).  
- Agrupaciones por país, tipo de actividad y tipo de ataque.  
- Cálculo de **tasa de fatalidad por país**.  
- Visualización de resultados mediante gráficos de barras y distribución de actividades.  
- Identificación de mercados más rentables para una aseguradora marítima.  

---

## 📊 Datos
- Fuente: [Global Shark Attack File](https://www.sharkattackfile.net/spreadsheets/GSAF5.xls)  
- Columnas clave:  
  - `date`, `type`, `country`, `activity_group`, `sex`, `age`, `fatal_y/n`, `species`  

---

## 🧹 Limpieza de datos
- Se estandarizaron nombres de especies y se agruparon en categorías principales.  
- Se eliminaron valores irrelevantes o desconocidos (`unknown`, registros inválidos).  
- La columna `age` se limpió, eliminando caracteres no numéricos y filas inconsistentes.  

---

## 🔍 Análisis realizado

### 1️⃣ Encuentros por país
- Países con más registros: **EEUU, Australia, Sudáfrica**.  
- Gráfico:  

![Encuentros por país](images/encuentros_por_pais.png)

---

### 2️⃣ Tasa de fatalidad por país
- Se calcula como:
  
Tasa Fatalidad (%) = (Fatal (Y) / Total encuentros) * 100

- Gráfico ordenado **ascendente por tasa de fatalidad**:  

![Tasa de fatalidad por país](images/fatalidad_por_pais.png)

---

### 3️⃣ Encuentros por actividad
- Actividades más frecuentes: **surfing, swimming, fishing**.  
- Gráfico:  

![Encuentros por actividad](images/encuentros_por_actividad.png)

---

## 💡 Conclusiones para aseguradora marítima
- **Mercados clave para seguros:**  
- 🇺🇸 EEUU, 🇳🇿 Nueva Zelanda, 🇫🇯 Fiji → volumen alto, riesgo moderado.  
- **Mercados a evitar:**  
- 🇮🇹 Italia → pocos seguros potenciales, tasa de mortalidad alta.  
- Datos útiles para diseñar estrategias de marketing, precios y productos según actividad y país.  

---

## ⚙️ Uso
1. Clonar el repositorio:  
```bash
git clone <repo-url>
