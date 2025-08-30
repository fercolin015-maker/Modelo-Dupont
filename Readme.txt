# 📊 Modelo DuPont en Streamlit

Este proyecto implementa un **modelo DuPont** en Python usando **Streamlit**.  
Permite analizar la rentabilidad de negocios a través de indicadores financieros clave, cargando datos desde archivos CSV o Excel.

## ✨ Funcionalidades

- Carga de archivos **.csv** o **.xlsx** con información financiera.
- Cálculo automático de:
  - **Margen Neto (%)**
  - **Rotación (veces)**
  - **Apalancamiento (veces)**
  - **ROE (%)**
  - **ROA (%)**
  - **Pay Back Capital (veces)**
  - **Pay Back Activos (veces)**
- Reporte en formato tabular:
  - **Columnas** = Períodos
  - **Filas** = Indicadores
- Descarga del reporte en **Excel**.

---

## 📂 Estructura del repositorio

```
├── app.py              # Código principal en Streamlit
├── README.md           # Instrucciones del proyecto
├── requirements.txt    # Librerías necesarias
└── data/
    └── ejemplo.xlsx    # Archivo de ejemplo con los datos de entrada
```

---

## 📥 Datos de entrada

El archivo debe contener al menos estas columnas:

| Periodo | Utilidad Neta | Ventas Netas | Activos Totales | Capital Contable |
|---------|---------------|--------------|-----------------|------------------|
| 2023    | 1000000       | 8000000      | 15000000        | 5000000          |
| 2024    | 1200000       | 9000000      | 16000000        | 5500000          |

---

## ⚙️ Instalación y uso local

1. Clona el repositorio:

```bash
git clone https://github.com/tu-usuario/modelo-dupont.git
cd modelo-dupont
```

2. Crea un entorno virtual (opcional pero recomendado):

```bash
python -m venv venv
source venv/bin/activate   # En Mac/Linux
venv\Scripts\activate      # En Windows
```

3. Instala dependencias:

```bash
pip install -r requirements.txt
```

4. Ejecuta la aplicación:

```bash
streamlit run app.py
```

5. Abre el navegador en [http://localhost:8501](http://localhost:8501)

---

## 🌐 Despliegue en Streamlit Cloud

También puedes desplegarlo gratis en [Streamlit Community Cloud](https://streamlit.io/cloud):

1. Sube tu repositorio a GitHub.
2. Conéctalo en Streamlit Cloud.
3. Selecciona `app.py` como archivo principal.
4. ¡Listo! 🚀

---

## 🧾 Licencia

Este proyecto está bajo la licencia MIT - consulta el archivo LICENSE para más detalles.
