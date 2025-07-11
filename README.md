Predicción de Enfermedades Cardíacas con Flask y Machine Learning

Aplicación web desarrollada con Flask que permite predecir el riesgo de enfermedad cardíaca a partir de dos variables: el porcentaje de la población que monta bicicleta y el porcentaje de fumadores. Usa un modelo de Machine Learning entrenado localmente y almacena predicciones por usuario.

---
 Tecnologías

- Python 3
- Flask
- Flask-SQLAlchemy
- Flask-Login
- Scikit-learn
- NumPy
- SQLite
- Bootstrap 5 (frontend)

---

Instalación y ejecución

# 1. Clona o descarga este repositorio

```bash
git clone https://github.com/tuusuario/proyecto_final_flask.git
cd proyecto_final_flask
```

### 2. Crea un entorno virtual (opcional pero recomendado)

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate   # Windows
```

### 3. Instala las dependencias

```bash
pip install -r requirements.txt
```

### 4. Genera el modelo predictivo (solo la primera vez)

```bash
python crear_modelo.py
```

Esto generará el archivo `models/model.pkl` necesario para las predicciones.

### 5. Ejecuta la aplicación

```bash
python app.py
```

Abre tu navegador en: [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

Funcionalidades

- Registro y login de usuarios
- Predicción personalizada usando ML
- Almacenamiento histórico por usuario (SQLite)
- Interfaz responsive con Bootstrap
- API REST (`/api/predict` y `/api/history`)

---

 Estructura del Proyecto

```
proyecto_final/
├── app.py
├── crear_modelo.py
├── requirements.txt
├── models/
│   └── model.pkl
├── templates/
│   ├── index.html
│   ├── login.html
│   └── register.html
└── database.db (se crea automáticamente)
```

---

