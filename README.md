# RP Platform - Sistema de Gestión de Servidores Roleplay

Una plataforma web completa para la gestión de servidores de Roleplay, construida con Next.js, Tailwind CSS y Supabase.

## 🚀 Características

### 🎮 Gestión de Usuarios y Roles
- Sistema de roles dinámicos estilo Discord
- Jerarquía de permisos numéricos (0-100)
- Panel visual de asignación de roles
- Autenticación segura con Supabase

### 👥 Sistema de Personajes (DNI)
- Múltiples personajes por usuario
- Historial médico y antecedentes penales
- Sistema de huellas digitales
- Generador visual de DNI

### 💰 Economía Completa
- Cuentas bancarias múltiples
- Transferencias en tiempo real
- Tarjetas de crédito/débito
- Control de inflación

### 🏪 Negocios y Propiedades
- Sistema de gestión de negocios
- Empleados con roles internos
- Control de stock e ingresos
- Mercado de propiedades

### 🎒 Inventario Avanzado
- Sistema basado en peso/espacio
- Items con durabilidad
- Inventario para personajes, vehículos y propiedades

### 🚔 CAD/MDT Policial y Médico
- Buscador de personajes con animaciones
- Sistema de multas y sanciones
- Historial médico completo
- Ordenes de búsqueda

### 🏦 Banca Web
- Dashboard estilo banco moderno
- Transferencias instantáneas
- Gráficos de gastos
- Pago de impuestos

### 📊 Panel de Administración
- Métricas en tiempo real
- Logs de acciones completos
- Sistema de reportes
- Gestión de sanciones

## 🛠️ Stack Tecnológico

- **Frontend**: Next.js 14 (App Router)
- **Estilos**: Tailwind CSS + Glassmorphism
- **Animaciones**: Framer Motion
- **Backend**: Supabase (PostgreSQL)
- **Autenticación**: Supabase Auth
- **Realtime**: Supabase Realtime
- **Gráficos**: Recharts
- **Iconos**: Lucide React
- **UI Components**: Radix UI + shadcn/ui

## 📋 Requisitos

- Node.js 18+ 
- npm o yarn
- Cuenta de Supabase

## 🚀 Instalación

1. **Clonar el repositorio**
```bash
git clone <repository-url>
cd RP-SISTEMS
```

2. **Instalar dependencias**
```bash
npm install
```

3. **Configurar variables de entorno**
```bash
cp .env.local.example .env.local
```
Editar `.env.local` con tus credenciales de Supabase:
```
NEXT_PUBLIC_SUPABASE_URL=tu_url_de_supabase
NEXT_PUBLIC_SUPABASE_ANON_KEY=tu_clave_anon_de_supabase
```

4. **Configurar la base de datos**
- Ve a tu proyecto de Supabase
- Ejecuta el contenido del archivo `schema.sql` en el editor SQL
- Esto creará todas las tablas, políticas y datos iniciales

5. **Iniciar el servidor de desarrollo**
```bash
npm run dev
```

Abre [http://localhost:3000](http://localhost:3000) en tu navegador.

## 📁 Estructura del Proyecto

```
src/
├── app/                    # App Router de Next.js
│   ├── auth/              # Páginas de autenticación
│   ├── dashboard/         # Panel principal
│   ├── bank/              # Banca web
│   ├── cad/               # CAD/MDT
│   ├── businesses/        # Gestión de negocios
│   └── admin/             # Panel de administración
├── components/            # Componentes React
│   ├── ui/               # Componentes UI base
│   ├── dashboard/        # Componentes del dashboard
│   ├── auth/             # Componentes de autenticación
│   └── forms/            # Formularios reutilizables
├── lib/                  # Utilidades y configuración
│   ├── supabase/         # Cliente de Supabase
│   └── utils/            # Funciones helper
├── types/                # Definiciones TypeScript
├── hooks/                # Custom hooks
└── utils/                # Utilidades varias
```

## 🗄️ Esquema de Base de Datos

El esquema completo se encuentra en `schema.sql` e incluye:

- **Usuarios y Roles**: Sistema de permisos granular
- **Personajes**: Múltiples personajes por usuario con DNI
- **Economía**: Cuentas bancarias, transferencias, tarjetas
- **Negocios**: Gestión completa de negocios y empleados
- **Inventario**: Sistema de items con peso y durabilidad
- **Licencias**: Múltiples tipos con estados
- **Logs**: Registro completo de acciones del sistema

## 🔐 Seguridad

- Row Level Security (RLS) en todas las tablas
- Políticas de acceso granulares
- Autenticación segura con Supabase
- Validación de inputs en frontend y backend
- Protección contra XSS y CSRF

## 📱 Mobile-First

El diseño está optimizado para dispositivos móviles:
- Layout responsive
- Touch-friendly
- Performance optimizada
- PWA ready

## 🎨 UI/UX

- Glassmorphism effects
- Animaciones fluidas con Framer Motion
- Transiciones de página suaves
- Notificaciones toast
- Loading states
- Dark theme por defecto

## 🚀 Despliegue

### Vercel (Recomendado)
1. Conecta tu repositorio a Vercel
2. Configura las variables de entorno
3. Despliega automáticamente

### Docker
```bash
docker build -t rp-platform .
docker run -p 3000:3000 rp-platform
```

## 📈 Monitoreo

- Métricas de usuarios online
- Control de economía (inflación)
- Logs de acciones en tiempo real
- Dashboard administrativo completo

## 🤝 Contribuir

1. Fork el proyecto
2. Crear una feature branch
3. Commit tus cambios
4. Push a la branch
5. Abrir un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT.

## 🆘 Soporte

Para reportar bugs o solicitar features:
- Abre un issue en GitHub
- Contacta al equipo de desarrollo

---

**RP Platform** - Transformando la gestión de servidores Roleplay 🎮
