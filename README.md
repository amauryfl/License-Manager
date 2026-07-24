# Software License Manager

Aplicación full stack para registrar y controlar licencias de software comercial.

## Funcionalidades

- React + Vite en el frontend.
- Backend Flask en Python.
- Base de datos SQLite creada automáticamente.
- Catálogo interno con 200 productos comerciales.
- Login mediante JWT.
- Contraseñas almacenadas con hash.
- Usuario inicial: `admin` / `admin`.
- Registro de licencias.
- Cálculo automático de licencias en uso y disponibles.
- Seguimiento de fecha de expiración.
- Comentarios por licencia.
- Imagen SVG automática para cada software.
- Registro de nuevos administradores.
- Solicitud de técnico de soporte mediante tickets.

## Ejecución local

### Backend

```bash
cd backend
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
python app.py
```

Backend:

```text
http://127.0.0.1:5000
```

### Frontend

```bash
cd frontend
npm install
copy .env.example .env
npm run dev
```

Frontend:

```text
http://localhost:5173
```

## Despliegue

- Subir `frontend/` a Vercel o Netlify.
- Subir `backend/` a Render, Railway o un servidor Python.
- Configurar `VITE_API_URL` con la URL pública del backend terminada en `/api`.
- Configurar `JWT_SECRET` y `FRONTEND_ORIGIN` en el backend.

