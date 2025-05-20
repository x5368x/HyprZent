# Guía PRO para Testers de HyprZent 🧪✨

¡Bienvenido/a al equipo de testers de **HyprZent**!  
Aquí tu curiosidad, tu ojo crítico y tus ganas de romper cosas para mejorar son el motor de nuestra evolución.  
Gracias a quienes testean, HyprZent es más robusto, usable y sorprendente con cada release.  
Esta guía te enseña cómo sacar todo el provecho a tu rol, colaborar fácilmente y reportar como un/a PRO.

---

## 🚀 Consigue la Última Versión de Desarrollo

Toda la innovación vive en la rama `dev`. Aquí se prueban funciones, correcciones y experimentos antes de llegar a producción.

### ¿Es tu primera vez?

1. Clona el repo oficial:
   ```bash
   git clone https://github.com/x5368x/HyprZent.git
   cd HyprZent
   ```
2. Cámbiate a la rama de desarrollo:
   ```bash
   git checkout dev
   ```

### ¿Ya tienes HyprZent clonado?

1. Actualiza `master` (producción):
   ```bash
   git checkout master
   git pull
   ```
2. Trae y entra a dev:
   ```bash
   git fetch origin dev
   git checkout dev
   git pull origin dev
   ```

---

## 🛠️ Instalación y Pruebas

Sigue el README para detalles, pero aquí tienes lo esencial:

- **Instalación completa:**
  ```bash
  ./install.sh
  ```
- **Solo restaurar dotfiles:**
  ```bash
  ./install.sh -r
  ```
- **Opciones del instalador:**
  ```bash
  ./install.sh [opciones]
      i : instalar Hyprland sin configs
      d : instalar Hyprland por defecto sin configs --noconfirm
      r : restaurar archivos de configuración
      s : habilitar servicios del sistema
      n : omitir acciones para Nvidia
      h : reevaluar el Shell
      m : saltar reinstalación de temas
      t : test run (simulación, no ejecuta cambios)
  ```

---

## 🔎 ¿Qué Probar? ¡Sé Creativo/a!

1. **Novedades:** ¿Las nuevas funciones realmente funcionan? ¿Se pueden romper?
2. **Interfaz y UX:** ¿Todo se ve bien y es intuitivo?
3. **Temas:** ¿Puedes cambiar entre claro/oscuro? ¿Algo falla?
4. **Fondos de pantalla:** ¿Cambian, se agregan o eliminan sin problemas?
5. **Características del sistema:** Notificaciones, atajos, configuraciones… ¿todo ok?
6. **Estabilidad:** ¿Se cuelga, crashea, hay glitches raros?
7. **Hardware variado:** Prueba en diferentes PCs, laptops o entornos virtuales.

---

## 🎯 ¿Qué Esperamos de tus Pruebas?

- **Aislamiento preciso:** Describe exactamente dónde, cuándo y cómo falla algo.
- **Evitar regresiones:** Asegúrate de que nada que funcionaba antes se rompió.
- **Experiencia real:** ¿Algo te incomoda? ¿Podría ser más intuitivo o rápido?
- **Rendimiento:** ¿Notas lags, alto consumo, procesos desbocados?

---

## 🦸 Privilegios y Reconocimiento para Testers PRO

- Tus reportes y sugerencias reciben atención prioritaria.
- Puedes opinar sin filtro: queremos sinceridad brutal y constructiva.
- Acceso anticipado a novedades, branches experimentales o previews.
- Ayudas a decidir el futuro de HyprZent: tu feedback define el rumbo.

---

## 🐞 Cómo Reportar Problemas como un/a PRO

### En GitHub (recomendado)

- Abre un issue o comenta en el PR de desarrollo:
  [Comparar dev/master (HyprZent)](https://github.com/x5368x/HyprZent/compare/master...dev)
- Usa la [plantilla de issues](.github/ISSUE_TEMPLATE) para estructurar tu reporte.

**Tips para un buen reporte:**
- Explica con detalle los pasos para reproducir el problema.
- Adjunta logs, capturas o videos si es posible.
- Especifica tu entorno: hardware, distro, drivers, etc.

### En Discord

- Usa el canal **#testers** para dudas rápidas, discusiones y coordinación.
- Los reportes formales, siempre en GitHub para que no se pierdan.

---

## 📅 ¿Cuándo se libera una nueva versión?

Consulta la [Política de Releases](./RELEASE_POLICY.md) para saber cuándo salen nuevas versiones y cómo puedes participar en los ciclos de pruebas finales.

---

## 🌱 Sé parte de la Comunidad

- Nadie cobra: aquí todos aportamos por pasión y aprendizaje.
- Cada sugerencia, reporte y test cuenta; ¡no subestimes tu impacto!
- Si tienes una idea loca, ¡compártela! A veces las mejores mejoras nacen del feedback menos esperado.

---

## 💧 Mantente HyprZentrado e hidratado

Gracias por probar, romper, sugerir, opinar y hacer de HyprZent el dotfile más cool de la comunidad Hyprland.  
¿Dudas? ¿Ideas? ¿Quieres sumarte al equipo?  
**¡Únete al Discord y haz historia con nosotros!**

---