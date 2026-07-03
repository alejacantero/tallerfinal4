# 🛍️ URBANA – Tienda de Moda

**URBANA** es un sitio web de e-commerce de moda desarrollado como proyecto front-end estático. Permite a los usuarios explorar colecciones de ropa, registrarse, iniciar sesión, gestionar su perfil y pedidos, y cuenta con un panel administrativo para la gestión de clientes.

## 🖼️ Vista previa

| Página principal | Panel de cliente | Panel administrativo |
|---|---|---|
| Landing con carrusel, colecciones y categorías | Perfil, métricas y pedidos | Gestión de clientes y métricas de la tienda |

## 🚀 Tecnologías utilizadas

- **HTML5** – Estructura semántica de las páginas.
- **[Bootstrap 5.3.3](https://getbootstrap.com/)** – Framework CSS para el diseño responsive (grid, componentes, utilidades). No se utilizó CSS personalizado adicional.
- **[Bootstrap Icons 1.11.3](https://icons.getbootstrap.com/)** – Iconografía utilizada en toda la interfaz.
- **JavaScript (vanilla)** – Interacciones puntuales (menú desplegable de género, alertas dismissibles).
- **CDN (jsDelivr)** – Todas las dependencias se cargan por CDN, sin necesidad de instalación ni build tools.

## 📁 Estructura del proyecto

```
urbana/
├── index.html              # Página principal (landing)
└── app/
    ├── login.html           # Inicio de sesión
    ├── registro.html        # Registro de nuevos usuarios
    ├── recuperar.html       # Recuperación de contraseña
    ├── cliente.html         # Panel del cliente
    └── admin.html           # Panel administrativo
```

## ✨ Funcionalidades por página

### `index.html` – Página principal
- Navbar responsive con menú de cliente.
- Carrusel de imágenes (Bootstrap Carousel).
- Banner de estadísticas de la marca.
- Cards de colecciones (Esencial, Trendy, Signature) con precios.
- Sección de categorías de productos.
- Sección "¿Por qué URBANA?".
- Formulario de contacto.
- Footer con enlaces de navegación y redes sociales.

### `app/login.html` – Inicio de sesión
- Formulario de acceso (correo y contraseña).
- Enlace a recuperación de contraseña.
- Enlace a registro para nuevos usuarios.
- Navbar y footer con acceso directo al inicio.

### `app/registro.html` – Registro
- Formulario completo de creación de cuenta (nombre, apellido, correo, teléfono, contraseña, género).
- Selector de género implementado con `dropdown` de Bootstrap (en lugar de `<select>` nativo, para una apertura más fluida).
- Checkbox de aceptación de términos y condiciones.
- Enlace a inicio de sesión.

### `app/recuperar.html` – Recuperar contraseña
- Formulario de recuperación por correo electrónico.
- Mensajes de estado (correo encontrado / no encontrado).
- Aviso para usuarios sin cuenta con enlace a registro.

### `app/cliente.html` – Panel del cliente
- Sidebar de navegación (oculto en móvil, con acceso alterno a "Salir").
- Alerta dismissible con acciones pendientes (envío y comprobante de pago).
- Tarjeta de perfil con foto, datos de contacto y estado de la cuenta.
- Tarjetas de métricas (pedidos activos, prendas compradas, total pagado, próxima entrega).
- Pestañas (`nav-tabs`) para alternar entre **Inscripciones Activas** e **Historial** de pedidos.
- Menú desplegable de usuario con acceso a Configuración y Cerrar sesión.

### `app/admin.html` – Panel administrativo
- Sidebar de administración con accesos a Clientes, Pedidos, Colecciones, Categorías, Inventario, Pagos y Configuración.
- Tarjetas de métricas generales de la tienda.
- Tabla de clientes registrados con estado de pedido y acciones (editar/eliminar).
- Modal de edición de cliente con formulario completo.

## 🎨 Diseño

Todo el diseño se construyó exclusivamente con clases utilitarias y componentes de **Bootstrap 5** (grid system, cards, navbar, carousel, tabs, modals, dropdowns, alerts, badges), sin hojas de estilo personalizadas adicionales. La paleta de la marca se basa en los colores predefinidos de Bootstrap: `dark`, `warning` (dorado) y `success` (verde), aplicados de forma consistente en todas las páginas.

## 📦 Cómo usarlo

No requiere instalación ni dependencias. Solo clona el repositorio y abre `index.html` en tu navegador:

```bash
git clone https://github.com/tu-usuario/urbana.git
cd urbana
```

Luego abre `index.html` directamente en tu navegador, o sirve la carpeta con cualquier servidor estático, por ejemplo:

```bash
npx serve .
```

## 📌 Notas

- Este proyecto contiene datos de ejemplo (clientes, pedidos, colecciones); no incluye backend ni base de datos.
- Los formularios (login, registro, recuperación, contacto) no tienen lógica de envío real; están listos para integrarse con un backend.


