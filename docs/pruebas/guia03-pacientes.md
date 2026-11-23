# Pruebas unitarias del módulo Pacientes (Guía 03)

Fecha: 23/11/2026 · Responsable: Bruno Pauccar

| Caso | Acción / Descripción | Resultado esperado | RF / RN | Resultado | Observación |
|------|----------------------|--------------------|---------|-----------|-------------|
| CP01 | Abrir /pacientes | 10 pacientes, total 40, «Siguiente »» | RF05 | OK | |
| CP02 | Buscar un DNI existente | Un solo paciente | RF05 | OK | |
| CP03 | Buscar parte de un apellido en minúsculas | Solo las coincidencias | RF05 | OK | |
| CP04 | Con búsqueda activa, ir a la página 2 | La URL conserva ?buscar= | RF05 | OK | |
| CP05 | Guardar el formulario vacío | Errores en español en los obligatorios | RF04 | OK | |
| CP06 | DNI de 7 dígitos | «exactamente 8 dígitos» y datos conservados | RF04 | OK | |
| CP07 | DNI de un paciente existente | «Ya existe un paciente…» | RN01 | OK | |
| CP08 | Fecha de nacimiento futura | «no puede ser futura» | RF04 | OK | |
| CP09 | Celular 812345678 | «debe empezar con 9» | RF04 | OK | |
| CP10 | Registrar un paciente válido | Ficha con aviso verde; total 41 | RF04 | OK | |
| CP11 | Editar solo el celular | Sin error de DNI; aviso verde | RF06 | OK | |
| CP12 | Editar con el DNI de otro paciente | «Ya existe un paciente…» | RF06, RN01 | OK | |
| CP13 | Eliminar un paciente con citas | Aviso rojo; sigue existiendo | RF07 | OK | |
| CP14 | Eliminar el paciente del CP10 | Aviso verde; total 40 | RF07 | OK | |
| CP15 | Abrir /pacientes/99999 | Página 404 | RF05 | OK | |