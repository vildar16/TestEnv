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

