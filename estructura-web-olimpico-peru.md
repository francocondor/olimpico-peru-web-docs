---
site:
  name: "Olímpico Perú"
  type: "Sitio web de academia deportiva"
  platform: "WordPress"
  builder: "Elementor"
  language: "es"
  year: 2025
  goal: "Presentar la academia, captar inscripciones y mostrar servicios/programas."
instructions:
  description: |
    Este archivo sirve como guía y registro del desarrollo de la web "Olímpico Perú".
    Cada sección representa una página o bloque principal del sitio.
    Puedes actualizar el estado de cada página (por ejemplo: pendiente, en progreso, terminado) y añadir notas sobre avances, cambios o tareas pendientes.
  usage:
    - Marca el estado de cada página usando la propiedad "status".
    - Añade comentarios o notas en la propiedad "notes" para cada página.
    - Actualiza el contenido y widgets conforme avances en el desarrollo.
  example:
    - page: "Inicio"
      status: "terminado"
      notes: "Slider y testimonios listos, falta optimizar CTA."
    - page: "Nosotros"
      status: "en progreso"
      notes: "Falta agregar fotos del equipo."
---

# Mapa Final de Estructura Web Olímpico Perú

## Progreso de desarrollo
pages:
  - name: "Inicio"
    status: "pendiente"
    notes: ""
  - name: "Nosotros"
    status: "pendiente"
    notes: ""
  - name: "Programas"
    status: "pendiente"
    notes: ""
  - name: "Servicios"
    status: "pendiente"
    notes: ""
  - name: "Galería"
    status: "pendiente"
    notes: ""
  - name: "Contacto"
    status: "pendiente"
    notes: ""
  - name: "Footer"
    status: "pendiente"
    notes: ""


## 1. Inicio
type: page
widgets:
  - hero_slider: {title, subtitle, call_to_action}
  - section: {title: "¿Por qué elegirnos?", description, featured_links}
  - testimonials: {list: [alumnos, padres]}
  - actions: [inscribirse, ver_programas, contactar]


## 2. Nosotros
type: page
widgets:
  - section: {title: "¿Quiénes Somos?", history, evolution}
  - section: {title: "Misión y Visión", mission, vision}
  - values: {visual_list}
  - team: {founders, directors, coaches, photos, roles}


## 3. Programas
type: page
programs:
  - academia_formativa: {categories_by_age, schedule, price, signup_button}
  - escuela_arqueros: {levels, schedule, price, signup_button}
  - futbol_competitivo: {requirements, selection_process, schedule, price, signup_button}


## 4. Servicios
type: page
services:
  - academia_formativa: {link_to_program}
  - futbol_competitivo: {link_to_program}
  - escuela_arqueros: {link_to_program}
  - alquiler_cancha: {contact_or_reserve_button}
  - entrenamiento_adultos: {contact_button}
  - futbol_femenino: {contact_button}


## 5. Galería
type: page
gallery:
  - academia_formativa: {images, videos}
  - club_olimpico_peru: {images, videos}
  - equipo_competitivo: {images, videos}


## 6. Contacto
type: page
contact:
  - info: {phone, email, address, schedule}
  - form: {name, phone, email, message}
  - map: {location}
  - social: {whatsapp, instagram, facebook}


## 7. Footer (en todas las páginas)
type: section
footer:
  - address
  - social: {whatsapp, instagram, facebook}
  - legal_links: {terms_of_use, privacy_policy, contact}
