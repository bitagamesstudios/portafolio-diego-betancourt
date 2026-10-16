# Plan de inglés y desarrollo de software internacional — Octubre 2026

**Propietario:** Diego Francisco Betancourt Ruiz  
**Fecha de seguimiento:** 16 de octubre de 2026  
**Objetivo:** trabajo remoto desde Colombia para empresas de Estados Unidos o España como Web/Frontend Developer, Junior Flutter Developer, Junior Full-Stack (por verificar), Application Support o QA funcional.

## Estrategia
- Consolidar un portafolio demostrable y CV en inglés; seleccionar vacantes que contraten explícitamente desde Colombia.
- Estudiar inglés técnico y practicar entrevistas, presentaciones de proyectos, explicación de errores y reuniones.
- Utilizar Claude y ChatGPT como asistentes, verificando el código, las pruebas y la comprensión personal. No presentar habilidades como dominadas sin evaluación.

## Evidencia del inventario GitHub (auditoría parcial)
- Web: HTML, CSS y JavaScript (Floristería Calas; sitios de Amparo's).
- Flutter/Dart: `serviquinautos-plus`, con `pubspec.yaml` y `lib/main.dart`. Se observaron rutas por rol, Firebase inicializado y dependencias como Provider, mapas, HTTP y Socket.IO.
- SQL/PostgreSQL: `app-finanzas/db/finanzas_db_01_esquema.sql`, tablas, funciones, restricciones e índices.
- Node.js/Express: descritos en el README de `app-finanzas`; implementación no auditada.
- Despliegue y analítica: Cloudflare Pages y GA4/UTM documentados en `amparos-floristeria-web`.
- Python y Lua: tecnologías declaradas por el titular; dominio por comprobar.
- **Precaución:** dependencia o tecnología encontrada no demuestra dominio personal, implementación terminada ni aplicación desplegada.

## Aprendizaje de JavaScript
### Ejercicio 1 — comprensión
Se trabajó con `productos.find(...)`, arreglos, funciones, comparación estricta y acceso a propiedades. Respuestas correctas: 5/5.

### Ejercicio 2 — corrección de errores
Objetivo: que `consultarPrecio("Tulipanes")` devuelva `"Producto no encontrado"` sin lanzar un TypeError. En la entrega inicial no se añadió la validación. Tema pendiente: manejo de `undefined` mediante condiciones y retorno anticipado.

Solución didáctica:
```javascript
function consultarPrecio(nombre) {
  const producto = productos.find(item => item.nombre === nombre);
  if (!producto) {
    return "Producto no encontrado";
  }
  return producto.precio;
}
```
Pruebas esperadas: `Girasoles -> 65000`; `Tulipanes -> "Producto no encontrado"`.

### Clase 3 — en curso
- `if`, `else`, `>=` y operadores lógicos.
- Ejercicio activo: completar `if (!producto) { return "Producto no encontrado"; }`.
- **Estado:** sin entrega del ejercicio 3; no señalar como completado.

## Inglés técnico
- Diagnóstico escrito preliminar: Pre-A1/A1 inicial basado en cinco respuestas cortas; no es un examen formal ni estima conversación.
- Frases objetivo: “I am a web developer”, “I work with HTML, Python and Lua”, “I want to work remotely for an international company”.
- Vocabulario: `bug`, `fix`, `function`, `return`, `undefined`, `condition`, `debugging`.
- Frase práctica: “I found a bug in the product search function and fixed it by adding a validation.”

## Próximos pasos
- [ ] Resolver el ejercicio 3 de `if` / `return` sin copiar.
- [ ] Realizar prueba práctica de JavaScript creando una función y casos de prueba.
- [ ] Validar lectura y escritura de código Flutter/Dart y SQL.
- [ ] Actualizar el CV bilingüe y casos de estudio técnicos con evidencias.
- [ ] Practicar inglés 30–60 min diarios y entrevistas simuladas.
- [ ] Evaluar oportunidades en Get on Board, LinkedIn, Wellfound y Revelo con elegibilidad para Colombia.

> Este archivo es un registro de aprendizaje y no certifica un nivel Junior o Mid.
