Documentación Técnica: Sistema "Monedas de la Patria"
📋 Resumen Ejecutivo
Monedas de la Patria es una aplicación web completa desarrollada para la gestión de compra, venta y catalogación de monedas argentinas históricas. El sistema integra tres módulos principales en una interfaz unificada:

🏪 Módulo de Comercio: Catálogo interactivo de monedas con sistema de compra/venta

📚 Módulo Educativo: Historia completa de la moneda argentina

📧 Módulo de Comunicación: Sistema de envío de correos a clientes

🛠️ Stack Tecnológico Utilizado
Frontend
Tecnología	Versión	Propósito
HTML5	-	Estructura semántica de la aplicación
CSS3	-	Estilos, diseño responsive y animaciones
JavaScript (ES6+)	-	Interactividad y lógica de negocio
CSS Grid & Flexbox	-	Layouts modernos y responsivos
Características Técnicas
Arquitectura: Single Page Application (SPA)

Diseño: Mobile-first, responsive design

Almacenamiento: LocalStorage para datos temporales

Navegación: Sistema de pestañas sin recarga de página

Arquitectura del Sistema
Estructura de Componentes
text
Monedas de la Patria/
├── Header (Navegación principal)
├── Sección Comercio
│   ├── Catálogo de monedas (Grid layout)
│   ├── Panel de usuario
│   └── Sistema de transacciones
├── Sección Historia
│   ├── Contenido educativo
│   └── Línea de tiempo interactiva
├── Sección Correos
│   ├── Lista de clientes
│   ├── Editor de mensajes
│   └── Plantillas predefinidas
└── Footer (Redes sociales y información)
Flujo de Datos
Inicialización: Carga de datos mock en localStorage

Navegación: Cambio entre secciones sin recarga

Interacción: Event listeners para todas las acciones del usuario

Persistencia: Guardado de borradores y preferencias

Diseño y UX
Principios de Diseño
Consistencia: Paleta de colores unificada (azul corporativo, dorado numismático)

Accesibilidad: Contraste adecuado, textos legibles

Usabilidad: Navegación intuitiva, feedback visual inmediato

Responsive: Adaptable a dispositivos móviles y desktop

Paleta de Colores
css
--primary-blue: #1e3c72 → #2a5298 (gradiente)
--secondary-gold: #d4af37 → #ffd700 (gradiente)
--neutral-gray: #f8f9fa, #e9ecef, #dee2e6
--success-green: #28a745
--danger-red: #dc3545
Funcionalidades Principales
Módulo de Comercio
Función	Tecnología	Complejidad
Catálogo de monedas	CSS Grid, JavaScript	Media
Sistema de usuarios	LocalStorage, Modales	Media
Transacciones	Event handling, DOM manipulation	Media-Alta
Panel de resumen	Dynamic content update	Baja
Módulo Educativo
Función	Tecnología	Complejidad
Línea de tiempo	CSS Flexbox, Cards	Baja
Contenido histórico	HTML semántico	Baja
Navegación	Tab system	Baja
Módulo de Comunicación
Función	Tecnología	Complejidad
Gestión de contactos	JavaScript arrays	Media
Editor de correos	Form handling	Baja
Plantillas	Object literals	Baja
Simulación envío	setTimeout, Promises	Baja
Flujos de Usuario
Proceso de Compra
text
1. Seleccionar usuario → Modal de registro/login
2. Explorar catálogo → Grid de monedas con hover effects
3. Seleccionar moneda → Modal de operación
4. Confirmar transacción → Actualización de panel lateral
Proceso de Envío de Correos
text
1. Seleccionar destinatario(s) → Lista de clientes
2. Elegir plantilla → Prefill de asunto y cuerpo
3. Personalizar mensaje → Textarea editable
4. Confirmar envío → Modal de confirmación
5. Feedback → Modal de éxito/error
Responsive Design
Breakpoints
css
/* Mobile First */
.container { max-width: 100%; padding: 0 1rem; }

/* Tablet */
@media (min-width: 768px) {
  .container { max-width: 720px; }
  .commerce-content { flex-direction: row; }
}

/* Desktop */
@media (min-width: 1024px) {
  .container { max-width: 1200px; }
  .grid { grid-template-columns: repeat(4, 1fr); }
}
Patrones Responsive
Flexbox para layouts unidimensionales

CSS Grid para layouts bidimensionales

Media queries para adaptación específica

Unidades relativas (rem, %) para escalado

Configuración y Despliegue
Requisitos del Sistema
Navegador moderno (Chrome 60+, Firefox 55+, Safari 12+)

JavaScript habilitado

Conexión a internet (para fuentes y recursos externos)

Estructura de Archivos
text
proyecto/
├── index.html (Aplicación principal)
├── styles.css (Estilos unificados)
└── assets/
    ├── images/ (Logo, monedas)
    └── fonts/ (Tipografías)
Instrucciones de Instalación
Descargar todos los archivos en una carpeta

Abrir index.html en un navegador web

No se requiere servidor web (funciona con file://)
# web_monedas_patria
