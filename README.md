# analysis-ConnectaTel - Análisis de Clientes LATAM

Análisis de comportamiento de clientes de una empresa de telecomunicaciones en Latinoamérica. Datos de 2022-2024.

---

## 🎯 ¿De qué va?

Analicé datos de **4,000 clientes** de ConnectaTel para:
- Entender cómo usan el servicio (llamadas, mensajes, datos)
- Identificar por qué algunos clientes se van (11.6% churn)
- Proponer planes nuevos para retenerlos

---

## 📊 Lo que encontré

| Grupo | % Clientes | Churn | Acción |
|-------|-----------|-------|--------|
| Bajo uso | 25% | 15% 🔴 | Crear plan más barato |
| Uso medio | 55% | 10% 🟡 | Ofertas de upgrade |
| Alto uso | 20% | 8% 🟢 | Programa VIP |

**La clave:** Los que más usan el servicio son los que se quedan. Así que: **más uso = menos se van**.

---

## 🗂️ Estructura

```
├── README.md (este archivo)
├── requirements.txt
│
├── notebooks/
│   └── ConnectaTel_Analisis_Clientes.ipynb
│
├── data/
│   ├── plans.csv
│   ├── users_latam.csv
│   └── usage.csv
│
└── docs/
    └── ANALISIS_EJECUTIVO.md
```

---

## 🚀 Cómo ejecutar

### Opción 1: Google Colab (fácil)
1. Ve a [Google Colab](https://colab.research.google.com/)
2. Abre desde GitHub: pega la URL del repo
3. Ejecuta las celdas (Shift + Enter)

**Ventaja:** No necesitas instalar nada.

### Opción 2: En tu compu (local)
```bash
# Clonar el repo
git clone https://github.com/tu-usuario/conectatel-analysis.git
cd conectatel-analysis

# Instalar librerías
pip install -r requirements.txt

# Abrir Jupyter
jupyter notebook
```

---

## 📈 Datasets

### plans.csv
- Planes disponibles (Básico, Premium)
- Precio, minutos incluidos, GB incluidos

### users_latam.csv
- Info de clientes: edad, ciudad, plan, si se fueron o no
- 4,000 usuarios

### usage.csv
- Detalle de uso real en 2024
- 40,000 registros de llamadas y mensajes

---

## 🔍 Análisis que hice

1. **Limpieza de datos:** Arreglé valores faltantes, sentinelas, fechas raras
2. **Exploración:** Entendí la estructura y encontré problemas
3. **Segmentación:** Dividí clientes en 3 grupos por edad y uso
4. **Visualización:** Histogramas, boxplots, distribuciones
5. **Recomendaciones:** Qué hacer para retener clientes

---

## 💡 Conclusiones principales

✅ **Bajo uso = Alta deserción (15% churn)**
- Estos clientes no ven valor
- Solución: Plan Lite más barato

✅ **Alto uso = Muy leales (8% churn)**
- Son los que más ingresos generan
- Solución: Programa VIP con beneficios especiales

✅ **Usuarios outliers (consumo extremo)**
- ~10% de clientes consumen MUCHO
- Generan la mayoría de ingresos
- Hay que cuidarlos bien

---

## 🛠️ Librerías usadas

- **pandas** → manipular datos
- **numpy** → operaciones numéricas
- **matplotlib** → gráficos
- **seaborn** → visualizaciones bonitas

---

## 📝 Archivos importantes

- **Notebook:** Todo el análisis paso a paso
- **Análisis ejecutivo:** Hallazgos y recomendaciones para stakeholders
- **Datos:** Los 3 CSVs originales


**Nota:** Los datos son ficticios (creados para el análisis). El método es real y aplicable a cualquier empresa de telecomunicaciones.
