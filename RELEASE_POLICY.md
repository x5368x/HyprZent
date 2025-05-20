# Política de Releases y Manejo de Ramas 🚦

Nuestra estrategia de ramas y releases está diseñada para mantener la máxima calidad y agilidad en el desarrollo, permitiendo iteraciones rápidas sin comprometer la estabilidad de producción.

---

## 🌿 Estructura de Ramas

- **`dev` (desarrollo activo):**  
  Aquí se integran y prueban todas las nuevas funciones, mejoras y correcciones. Es la rama para el trabajo diario y colaborativo.

- **`master` (producción estable):**  
  Solo recibe código desde `dev` tras una validación exhaustiva. Representa siempre el estado publicado en producción.

- **`release` (snapshot de producción):**  
  Replica el estado de `master` en el momento de un release importante. No recibe cambios posteriores, solo sirve como referencia para soporte o auditoría.

---

## 📅 Ciclo de Releases Semanal (Flexible)

- **Congelación en `dev`:**  
  El avance en la rama `dev` se congela típicamente a mitad o final de semana (miércoles o jueves). Desde ese momento, solo se permiten correcciones críticas y pruebas finales.

- **Ventana de Release:**  
  El merge de `dev` en `master` y el despliegue a producción ocurren los viernes, con margen de maniobra para asegurar la calidad.

- **Etiquetado y Snapshots:**  
  En la primera y tercera semana del mes, se etiqueta el estado de `master` como release estable y se actualiza la rama `release` como histórico.

---

## 🕒 Flujo de Trabajo

| Día                      | Actividad                                             |
|--------------------------|------------------------------------------------------|
| Lunes–Miércoles          | Desarrollo activo y testing en `dev`                 |
| Jueves (congelación)     | Últimos ajustes y validación. Solo fixes urgentes.   |
| Viernes (release)        | Merge de `dev` a `master` y despliegue flexible      |
| Viernes–Domingo          | Monitoreo en producción, hotfixes si hace falta      |

---

## 🛠️ Desarrollo, Testing y Deploy

- **Inicio de semana:**  
  Se integran nuevas funcionalidades, mejoras y correcciones en `dev`. QA realiza validaciones continuas.

- **Jueves:**  
  Se congela el desarrollo en `dev`. El equipo se concentra en pruebas de regresión y validación final.

- **Viernes:**  
  Si todo está validado, `dev` se fusiona en `master` y se despliega a producción. El horario es adaptable según el avance.

- **Fin de semana:**  
  Se monitorea la producción. Si surge un problema crítico, se aplica hotfix directamente a `master` y, tras validación, se lleva a `dev`.

---

## 🔀 Pull Requests

- Todos los cambios deben proponerse a través de PRs contra `dev`.
- Cada PR requiere revisión y aprobación mínima de un desarrollador diferente al autor.
- Los PRs deben aceptarse y mergearse antes de la congelación semanal para entrar en la siguiente release.
- No se permiten merges directos a `master` ni a `release`.
- Los PRs pueden crearse en cualquier momento, pero deben ser revisados y aceptados en `dev` antes de la ventana de release.

---

## 📝 Consideraciones y Buenas Prácticas

- **Flexibilidad:**  
  Los horarios exactos de freeze y release pueden variar según la disponibilidad del equipo y la calidad del build. La prioridad es la estabilidad.

- **Comunicación clara:**  
  Cada semana se informará el calendario estimado y cualquier ajuste a través de canales internos de comunicación (ej: Discord, commits, etc.).

- **Evolución continua:**  
  Esta política es viva y puede ajustarse según la experiencia y las necesidades del equipo. Se agradece el feedback.

- **Sin fechas rígidas:**  
  No hay horas exactas; se prioriza la preparación del release sobre el calendario, ajustando tiempos según el contexto.

---

¿Tienes sugerencias o necesitas aclaraciones?  
¡Anímate a proponer mejoras mediante un PR o issue!