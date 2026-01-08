
# Ejemplo de proyecto ficticio

---

## Proyecto: **ReBootHub – Reutilización y reacondicionamiento de dispositivos**

### 1) Idea del producto/servicio

**ReBootHub** es un servicio digital que conecta:

* centros educativos,
* empresas,
* y organizaciones locales,

para **recolectar, reacondicionar y redistribuir** portátiles, tablets y PCs que ya no se usan, reduciendo el **e-waste** y la **brecha digital**.

**Qué problema aborda**

* Mucho hardware se desecha aunque todavía es reutilizable.
* Parte del alumnado no tiene acceso a equipos adecuados.
* El reacondicionamiento suele ser informal y sin trazabilidad.

**Qué ofrece**

* Un “circuito” claro: recogida → diagnóstico → reacondicionado → entrega → seguimiento.
* Un sistema de “trazabilidad” del dispositivo (historial de reparaciones y uso).
* Una guía de ecodiseño y mantenimiento para alargar la vida útil.

### 2) ODS vinculados (RA3.a)

* **ODS 12** (Producción y consumo responsables): reutilización, reparación, alargar vida útil.
* **ODS 4** (Educación de calidad): acceso a recursos digitales.
* **ODS 10** (Reducción de desigualdades): reducir brecha digital.
* (Opcional) **ODS 13** (Acción por el clima): menos emisiones al evitar fabricar equipos nuevos.

### 3) Riesgos y oportunidades (RA3.b)

**Oportunidades**

* Reducción de residuos electrónicos.
* Mejora de la inclusión digital.
* Ahorro económico para familias y centros.
* Imagen positiva y alianzas con empresas (RSC).

**Riesgos**

* Gestión de datos personales (borrado seguro).
* Coste del reacondicionado y logística.
* Falta de participación de empresas.
* Dispositivos obsoletos (compatibilidad y rendimiento).

### 4) Acciones sostenibles desde el rol profesional (RA3.c)

Acciones concretas “como desarrolladores”:

* Diseñar la web ligera (sin frameworks pesados), imágenes optimizadas.
* Asegurar accesibilidad (contraste, navegación teclado).
* Formularios simples: “donar equipo”, “solicitar equipo”, “voluntariado técnico”.
* Promover software libre y sistemas ligeros (Linux, herramientas de mantenimiento).
* Documentar procedimientos de borrado seguro y reacondicionado.

### 5) Economía circular (RA4.a–c)

**Modelo actual (clásico)**

* Comprar → usar → desechar.
* Reemplazo por moda o por falta de reparación.
* Residuos y extracción de materias primas.

**Economía circular**

* Reutilizar y reparar.
* Diseñar para durar.
* Mantener y reacondicionar.
* Dar “segunda vida” y trazabilidad.

**Beneficios**

* Menos residuos electrónicos.
* Menos extracción de recursos.
* Menos emisiones por fabricación/transporte.
* Más acceso equitativo a tecnología.

### 6) Ecodiseño aplicado (RA4.d)

Ecodiseño en el servicio:

* Reacondicionar con piezas reutilizadas siempre que sea seguro.
* Diseñar un proceso “estándar” de diagnóstico para evitar desperdicios.
* Manual de mantenimiento para prolongar vida útil.

Ecodiseño en la web:

* Pocas dependencias, CSS propio.
* Imágenes comprimidas (`.webp`).
* Tipografías del sistema (sin cargar Google Fonts).
* Sin vídeos pesados; si se usan, bajo demanda.

### 7) Ciclo de vida del producto/servicio (RA4.e)

Ejemplo de análisis (resumido):

1. **Entrada**: recepción del dispositivo (donación o retirada).
2. **Diagnóstico**: estado, piezas, batería, RAM/SSD.
3. **Reacondicionado**: limpieza, sustitución mínima, instalación.
4. **Distribución**: entrega a centro/alumnado con “kit” de uso responsable.
5. **Uso y soporte**: incidencias, mantenimiento anual.
6. **Fin de vida**: reutilización de piezas / reciclaje certificado.

---

## Modelo de web

### Estructura mínima (5 páginas)

* `index.html` (home)
* `pages/producto.html` (qué es ReBootHub)
* `pages/sostenibilidad.html` (ODS + riesgos/oportunidades + acciones del desarrollador)
* `pages/ciclo-vida.html` (economía circular + ciclo de vida)
* `pages/equipo.html` (quiénes somos + reparto de tareas)

### Boceto (wireframe) orientativo

**HOME (index.html)**

* Header con nav
* Hero: “Dale una segunda vida a la tecnología”
* 3 tarjetas: Donar / Solicitar / Ser voluntario
* Sección “Impacto” (números simulados: equipos recuperados, kg e-waste evitado…)
* Footer

**SOSTENIBILIDAD**

* Bloque ODS (iconos + explicación corta)
* Tabla “Riesgos / Oportunidades”
* Lista “Acciones sostenibles como desarrolladores”

**CICLO DE VIDA**

* Línea temporal del proceso (6 pasos)
* Comparativa “modelo clásico vs circular” (tabla)
* “Ecodiseño aplicado” (producto + web)

---

## Ejemplos de funcionalidades JavaScript (simples y viables)

El JS no tiene que ser complejo, pero sí útil. Por ejemplo:

1. **Formulario con validación**

* En “Donar equipo”: nombre, email, tipo de dispositivo, estado.
* Validar: campos obligatorios + email correcto.
* Mostrar un mensaje de confirmación.

2. **Acordeón / FAQ**

* Preguntas frecuentes (borrado de datos, requisitos, tiempos).

3. **Filtros**

* Filtrar “tipos de dispositivos aceptados” por estado (A/B/C).

4. **Contador de impacto (simulado)**

* Al pulsar “Calcular impacto”: mostrar estimación (ej. kg de CO₂ evitado) según el tipo de dispositivo.
* Esto encaja muy bien con sostenibilidad y es motivador.

---

## Cómo se repartiría el trabajo

Ejemplo para un grupo de 4 alumnos:

* Alumno A: `index.html` + CSS header/nav
* Alumno B: `producto.html` + sección impacto
* Alumno C: `sostenibilidad.html` + tabla riesgos/oportunidades
* Alumno D: `ciclo-vida.html` + timeline + tabla circular vs clásico
  **JS** lo hacen entre 2 (o uno coordina y los demás aportan).

---

## Ejemplos de commits “tipo diario”

* `feat: estructura inicial del proyecto y navegación`
* `add: contenido inicial de producto (qué es ReBootHub)`
* `style: layout responsive del header y tarjetas`
* `feat: formulario donar equipo con validación JS`
* `add: sección ODS y tabla riesgos/oportunidades`
* `add: timeline ciclo de vida + comparativa circular vs clásico`
* `fix: enlaces relativos y rutas de assets`
* `docs: actualizar README con reparto de tareas y enlace a Pages`

---
