# Convención de Commits

Utilizamos la siguiente convención para mantener un historial de commits claro, coherente y útil:

```
<tipo>[alcance opcional]: <mensaje corto>

[Descripción más larga opcional]
```

- Usa el **modo imperativo en presente**: _"agregar"_, _"corregir"_, no _"agregado"_, _"corrigió"_.
- El mensaje debe ser **breve y descriptivo**. Evita frases genéricas como _"cambios varios"_.

---

## Tipos permitidos

| Tipo     | Propósito                                                                 |
|----------|--------------------------------------------------------------------------|
| `feat`   | Nueva funcionalidad                                                       |
| `fix`    | Corrección de errores                                                     |
| `docs`   | Cambios en la documentación (README, comentarios, etc.)                  |
| `style`  | Cambios que no afectan la lógica (espacios, formato, etc.)               |
| `refactor` | Reestructuración del código sin cambiar funcionalidad                |
| `perf`   | Mejora de rendimiento                                                     |
| `test`   | Agregado o mejora de pruebas                                              |
| `chore`  | Tareas menores (builds, dependencias, configuraciones)                   |
| `ci`     | Cambios en la configuración de integración continua                      |
| `ui`     | Cambios en la interfaz grafica                     |

---

## Ejemplos prácticos

```bash
feat(auth): agregar login con Google
fix(api): corregir error 500 al crear usuario
docs(readme): actualizar instrucciones de instalación
style(controladores): formatear codigo del archivo
refactor(db): separar lógica de conexión en archivo aparte
```

---

# Convención de código

Utilizamos la siguiente convención para mantener un orden y misma estructuración en el código:

- Usa formato **camelCase** en variables: no hay espacio entre palabras, empieza en minuscula y cada nueva palabra (después de la primera) comienza con una letra mayúscula. Ejemplos: totalInventario, nombreObjeto, tipoSalida...

- Formato mayuscula para **constantes**. Ejemplo: VALOR_MAX, VALOR_MIN

## 📌 Convención por tipo

| Tipo de variable   | Ejemplo       | Convención             |
|--------------------|---------------|-------------------------|
| Booleano           | `isActive`    | Prefijo `is`, `has`     |
| Contador/Índice    | `i`, `j`      | Permitido en bucles     |
| Objeto o Variable            | `userProfile` | `camelCase`             |
| Array              | `userList`    | `camelCase` y plural    |
| Constante global   | `MAX_LIMIT`   | MAYÚSCULAS              |


## 📌 Comentarios descriptivos antes de cada función


/**
 * [Breve descripción de la función: qué hace y por qué existe]
 *
 * @param {tipo} nombre - Descripción del parámetro
 * @param {tipo} nombre - Descripción del parámetro (si hay más)
 * @returns {tipo} - Qué devuelve la función (si aplica)
 */

 Ejemplo:

 /**
 * Calcula el precio total con impuesto incluido.
 *
 * @param {number} precio - Precio base del producto
 * @param {number} impuesto - Porcentaje de impuesto a aplicar (0.0 - 1.0)
 * @returns {number} - Precio final con impuesto
 */