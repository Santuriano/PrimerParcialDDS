# 🎓 Sistema de Estudio — Parcial 1 · Desarrollo de Software

Sistema de estudio **acelerado** para preparar el **Primer Parcial de Desarrollo de Software** (UTN-FRC). Es una aplicación web de una sola página, autocontenida en el archivo [`index.html`](index.html): no necesita instalación, ni servidor, ni paso de *build*. Se abre directamente en el navegador.

> **Filosofía 80/20:** se estudia con **recuerdo activo** (reproducir de memoria) y **repetición espaciada** en lugar de releer pasivamente, priorizando los temas que más rinden en un examen situacional. Plan de arranque desde cero: **6 días · 3 h/día**.

---

## 🚀 Cómo usarlo

1. Descargá o cloná este repositorio.
2. Hacé doble clic en [`index.html`](index.html) (o abrilo con tu navegador).
3. ¡Listo! No hay nada que instalar ni compilar.

```bash
git clone https://github.com/Santuriano/PrimerParcialDDS.git
cd PrimerParcialDDS
# Abrí index.html en tu navegador
```

> 💡 Con conexión a internet carga las tipografías de Google Fonts; sin conexión funciona igual usando las fuentes del sistema. El progreso de la pestaña **Repaso** se guarda en tu navegador (`localStorage`).

---

## 🧭 Secciones

La app se organiza en **4 pestañas** navegables desde la barra superior (*sticky*):

| Pestaña | Contenido |
|---------|-----------|
| 🗓️ **Plan** | Plan de estudio de **6 días** (3 h/día) con un diagnóstico 80/20 que marca los temas de mayor peso y, para cada día, objetivos + una consigna de **recuerdo activo**. |
| 🃏 **Fichas** | **42 tarjetas** de recuerdo activo con efecto de *giro*, filtro por categoría, mezcla aleatoria y navegación anterior/siguiente. Pensás la respuesta **antes** de dar vuelta la ficha. |
| ✅ **Simulacro** | **37 preguntas** estilo parcial: opción simple, **multi-respuesta** y **relacionar** (*matching*). Modo completo o express (10 al azar), con autocorrección, justificación docente y nota aproximada /10. |
| 🔁 **Repaso** | Tabla de **repetición espaciada**: marcás cada tema en 3 momentos (1ª vuelta · +2 días · pre-examen) y señalás los temas **débiles**. Se guarda en el dispositivo. |

---

## 📘 Temario cubierto (Apuntes 01 → 14)

| Apunte | Tema |
|--------|------|
| **01–02** | Stack en capas (Cliente · Frontend · Backend · Database), Full Stack, qué **no** puede hacer JS en el navegador (*Same Origin Policy*) y **Git** (estados, `add`/`commit`/`push`/`pull`, ramas, `.gitignore`). |
| **03** | **HTML**: estructura, etiquetas semánticas vs `div` y formularios (`label`/`for`, `action`/`method`). |
| **04–05** | **CSS**: regla, selectores y modelo de cajas (content · padding · border · margin) + **Bootstrap** (grid responsive, CDN). |
| **06** | **JavaScript I**: tipos, tipado dinámico, `==` vs `===` (coerción), *falsy*, funciones, *hoisting* y *arrow functions*. |
| **07** | **JavaScript II**: objetos, arrays (`map`/`filter`/`forEach`/`find`), *destructuring*, módulos y JSON. |
| **08** | **DOM / SPA**: árbol del DOM, `getElementById`, `textContent`/`innerHTML`, eventos, `addEventListener` y *hash routing*. |
| **09** | **Node / NPM**: entorno de ejecución V8, *single-thread* + *event loop*, `package.json`, `dependencies` vs `devDependencies`. |
| **10** | **Asincronía**: callbacks, `setTimeout`, promesas (`then`/`catch`), `async`/`await`, `fetch` y la colección `Map`. |
| **11** | **ORM / Sequelize**: modelo = tabla, validación vs restricción y CRUD (`findAll`/`findOne`/`create`/`bulkCreate`). |
| **12** | **Arquitectura / HTTP**: REST (cliente-servidor, sin estado), métodos HTTP y códigos de estado (incluido el clásico **401 vs 403**). |
| **13–14** | **Express / Router**: `app.{método}(path, handler)`, `req` (params/query/body), `res` (send/json/status), `Router`, `static` y **CORS**. |

---

## ✨ Características

- **Recuerdo activo:** las fichas se *dan vuelta* al tocarlas; predecís la respuesta antes de verla.
- **Filtros por categoría:** 11 categorías (Fundamentos, Git, HTML, CSS/Bootstrap, JS, DOM/SPA, Node/NPM, Asincronía, ORM/Sequelize, Arquitectura/HTTP, Express).
- **Simulacro autoevaluable:** corrección automática con aciertos/errores marcados, explicación de cada respuesta y puntaje con nota estimada.
- **Tres tipos de pregunta:** opción simple, multi-respuesta y relacionar — igual que en el examen.
- **Repetición espaciada con persistencia:** la tabla de repaso recuerda tu progreso entre sesiones (`localStorage`).
- **Diseño responsive:** tema oscuro, navegación adhesiva y layout adaptable a celular y escritorio.

---

## 🛠️ Tecnología

- **HTML5**, **CSS** puro (variables CSS, tema oscuro) y **JavaScript** *vanilla*.
- **Cero dependencias**, sin frameworks, sin paso de *build* y sin backend.
- Tipografías de **Google Fonts** (Spectral, Inter, JetBrains Mono) con *fallback* a fuentes del sistema.
- Todo el contenido (estilos, datos y lógica) vive dentro de un único archivo [`index.html`](index.html), por lo que es 100% portable.

---

## 📂 Estructura del proyecto

```
PrimerParcialDDS/
├── index.html   # La aplicación completa (HTML + CSS + JS)
└── README.md    # Este archivo
```

---

## 📄 Licencia

Material de estudio de uso libre con fines educativos.
