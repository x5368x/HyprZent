# Guía PRO para Mensajes de Commit 🚀

Un historial de commits impecable es la mejor carta de presentación para cualquier proyecto. Es la base para entender la evolución del código, facilitar revisiones, encontrar errores y colaborar de forma eficiente. Si quieres que tu repo sea mantenible y profesional, dedica tiempo a tus mensajes de commit.

---

## ⭐ Principios Clave

1. **Un commit, un propósito:**  
   Cada commit debe ser atómico. Si estás cambiando dos cosas distintas, haz dos commits.

2. **El mensaje es tu legado:**  
   Escribe para tu yo del futuro y para tus compañeros. Explica el _qué_, el _por qué_ y, cuando sea relevante, el _cómo_ del cambio.

3. **Los mensajes cortos salvan vidas:**  
   El resumen debe ser breve (máx. 50 caracteres). Si hay más que decir, expándelo en el cuerpo.

4. **El primer renglón, en modo imperativo:**  
   Ejemplo:  
   - ✅ `Agrega validación de emails`  
   - ❌ `Agregando validación de emails`  
   - ❌ `Agregado validación de emails`  

5. **Líneas cortas, historia legible:**  
   Envuelve el cuerpo a 72 caracteres por línea.

6. **Haz referencia a issues y tareas:**  
   Ejemplo: `Closes #123`, `Refs #45`

---

## 📝 Estructura Recomendada

```
<tipo>(opcional: alcance): resumen corto en modo imperativo

(Cuerpo opcional: Explica el contexto, motivo, impacto, limitaciones, etc.
Incluye referencias a issues o pull requests si aplica.)

Ejemplo:
feat(auth): permite login con Twitter

Se añadió la autenticación vía OAuth para Twitter. El usuario puede conectar
su cuenta y acceder con un solo clic. Refs #22
```

---

## 🏷️ Tipos de Commit (prefijos convencionales)

| Tipo        | Para qué usarlo                                           | Ejemplo                                         |
|-------------|----------------------------------------------------------|-------------------------------------------------|
| `feat`      | Nueva funcionalidad                                      | `feat: agrega modo oscuro`                      |
| `fix`       | Corrección de bugs                                       | `fix: evita crash al subir PDF`                 |
| `docs`      | Cambios en documentación                                 | `docs: aclara uso del archivo settings.yml`     |
| `style`     | Cambios de formato/estilo (sin afectar lógica)           | `style: reordena imports en api.py`             |
| `refactor`  | Refactorización sin cambio de funcionalidad              | `refactor: simplifica lógica de rutas`          |
| `test`      | Añade o corrige tests                                    | `test: testea caso límite en parser`            |
| `chore`     | Tareas de mantenimiento (deps, scripts, configs, etc.)   | `chore: actualiza dependencias`                 |
| `perf`      | Mejoras de rendimiento                                   | `perf: optimiza renderizado en móvil`           |
| `ci`        | Integración continua (GitHub Actions, Travis, etc.)      | `ci: corrige nombre de workflow`                |
| `build`     | Cambios de build, empaquetado, dependencias              | `build: actualiza versión de node`              |
| `security`  | Cambios de seguridad                                     | `security: elimina XSS en comentarios`          |
| `merge`     | Fusión de ramas                                          | `merge: integra rama develop`                   |
| `revert`    | Reversión de un commit                                   | `revert: revierte feat: login con Twitter`      |
| `config`    | Cambios en archivos de configuración                     | `config: ajusta eslint para nuevos estándares`  |
| `deploy`    | Modificaciones en despliegue                             | `deploy: automatiza subida a Netlify`           |
| `init`      | Primer commit / inicialización de proyecto               | `init: estructura base del proyecto`            |
| `move`      | Movimiento de archivos/directorios                       | `move: traslada assets a public/`               |
| `rename`    | Renombrar archivos, carpetas, variables, etc.            | `rename: renombra UserController a AuthCtrl`    |
| `remove`    | Eliminaciones (archivos, código, dependencias)           | `remove: elimina tests obsoletos`               |
| `update`    | Cambios varios menores (usa con moderación)              | `update: actualiza ejemplos en README`          |

> **Personaliza los tipos si tu equipo lo necesita, pero documenta y usa siempre los mismos.**

---

## 🖋️ Consejos PRO

- **Evita “fixes”, “updates”, “varios”, “ajustes”, etc. sin contexto.**  
  Sé específico.
- **Haz commits pequeños y frecuentes.**  
  Es más fácil revertir y entender cada cambio.
- **No subas commits con contenido no relacionado.**  
  (Por ejemplo, no mezcles cambios de dependencias y de lógica en uno solo.)
- **Prefiere el español si tu equipo lo prefiere, pero sé coherente.**
- **Incluye siempre referencias automáticas a issues o PRs cuando corresponda.**

---

## 💡 Plantilla universal

```
<tipo>(opcional: alcance): resumen breve en imperativo

(Explicación detallada si es necesario, contexto, motivo, referencias…)

Refs #xx / Closes #yy
```

---

## 📚 Recursos Recomendados

- [Conventional Commits (ES)](https://www.conventionalcommits.org/es/v1.0.0/)
- [Cómo escribir un buen mensaje de commit (ES)](https://cbea.ms/git-commit/)
- [Guía Angular Commit Message](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#commit)

---

¿Dudas o sugerencias?  
¡Propón tus cambios en este archivo vía Pull Request!  
Haz de tu historial de commits una obra de arte digital.