# 🚀 Cómo trabajar en equipo en Venus-Project

Guía rápida, sin comandos. Usamos **GitHub Desktop**, un programa con botones, y Unreal Engine 5.5.

> ⚠️ **Lo único importante:** los Blueprints y mapas no se pueden mezclar. Si dos personas editan **el mismo archivo**, una pierde su trabajo. Por eso: **cada uno trabaja en lo suyo y avisa si va a tocar algo de otro.**

---

## 🛠️ Primera vez (15 minutos)

1. Bajá e instalá [GitHub Desktop](https://desktop.github.com) e iniciá sesión con tu cuenta de GitHub.
2. Aceptá la invitación al proyecto (te llega por mail).
3. En GitHub Desktop: **File → Clone repository → Venus-Project → Clone**.
   Tarda un rato, el proyecto pesa ~800 MB ☕
4. Abrí la carpeta clonada y hacé doble clic en **Venus001.uproject** (con Unreal 5.5).
   La primera vez tarda en preparar todo. Es normal.

---

## 📅 Cada vez que te ponés a trabajar

**1. Cerrá Unreal** (si lo tenés abierto).

**2. Traé lo último**
Arriba en GitHub Desktop: **Current branch → main**, y después **Fetch origin / Pull origin**.

**3. Creá tu rama** (tu copia de trabajo)
**Current branch → New branch** y ponele nombre a lo que vas a hacer, por ejemplo `enemigo-alien` o `nave-movimiento`.

**4. Abrí Unreal y trabajá** 🎮

---

## 💾 Cuando terminás

1. **Guardá todo en Unreal** (Ctrl + Shift + S) y cerralo.
2. En GitHub Desktop vas a ver la lista de cambios a la izquierda.
   - ✅ Tiene que aparecer **solo lo que tocaste vos**.
   - 🤔 Si aparece algo raro que no tocaste, **no lo subas** y preguntá.
3. Abajo a la izquierda, escribí qué hiciste en una frase (ej: *"Agrego movimiento del alien"*) y tocá **Commit**.
4. Tocá **Publish branch** (o **Push origin**).
5. Tocá **Create Pull Request**. Se abre GitHub: poné un título y confirmá.
6. Avisá al grupo. Alguien lo revisa y lo une al proyecto principal. ¡Listo! 🎉

---

## 🤝 Reglas para no pisarnos

- 🧍 **Cada uno es dueño de sus Blueprints.** No edites el de otro sin avisar.
- 🗺️ **Los mapas los toca una persona a la vez.** Para probar cosas, usá tu propio mapa.
- 📢 **Antes de abrir algo compartido (mapa, Blueprint de otro), avisá en el grupo:** *"Estoy tocando Nave.umap"*. Y avisá también cuando termines.
- 🚫 **No renombres ni muevas archivos compartidos** sin avisar. Les rompe el proyecto a los demás.
- 🌿 **No trabajes en `main`.** Siempre en tu rama.
- 🪙 **Guardá seguido:** commits chicos, con mensajes que se entiendan.

---

## 🆘 Si algo sale mal

| Problema | Qué hacer |
|---|---|
| Aparecen archivos que no toqué | No los subas. Preguntá. |
| "Hay cambios sin guardar" al cambiar de rama | Hacé Commit primero, o preguntá antes de descartar. |
| Hay un conflicto en un `.uasset` o `.umap` | **No intentes arreglarlo solo.** Avisá: hay que elegir una de las dos versiones. |
| Unreal pide un plugin que no tengo | Avisá. No lo agregues vos. |
| Quiero deshacer lo que cambié en un archivo | Clic derecho sobre el archivo → **Discard changes**. ⚠️ No se puede recuperar. |
| Un archivo aparece de solo lectura | Alguien lo tiene bloqueado. Preguntale en el grupo. |

---

## ℹ️ Bueno saber

- Las carpetas `Binaries`, `Intermediate`, `Saved` y `DerivedDataCache` las genera Unreal en cada compu y **no se suben**. Si las ves en la lista de cambios, avisá.
- ¿Sos de usar comandos? Podés usar `git` normal, pero necesitás **Git LFS** instalado (`git lfs install`) antes de clonar.
- 🔒 **Bloqueo de archivos (opcional, solo con comandos):** `git lfs lock <archivo>` bloquea un asset para que nadie más lo edite, y `git lfs unlock <archivo>` lo libera. En el día a día alcanza con avisar en el grupo.
