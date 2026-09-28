# MP5021 · Incidentes de Ciberseguridad — web del módulo

Web didáctica del módulo **MP5021 Incidentes de Ciberseguridade** (Curso de Especialización, IES Chan do Monte, 2026/2027). Dos versiones generadas de una misma fuente, en HTML autocontenido (sin dependencias que compilar).

| Fichero | Versión | URL al desplegar |
|---|---|---|
| `index.html` | **Alumnado** — sin soluciones ni notas docentes | `/` |
| `profesorado/index.html` | **Profesorado** — todo + correcciones, decisiones y resumen operativo | `/profesorado/` |

Incluye laboratorio (Proxmox en aula + Vagrant en casa, red `172.21.10.0/24`, Debian 12), teoría por unidad, las 26 actividades con su capa de IA (ruta · riesgo · control) y la evaluación. Interruptor de "Capa IA" y tema claro/oscuro incorporados.

## Desplegar en Netlify (rápido)
1. Entra en app.netlify.com → **Add new site → Deploy manually**.
2. Arrastra **esta carpeta** (o el .zip). Home = alumnado; profesorado en `/profesorado/`.

## Desplegar con GitHub + Netlify (auto-despliegue)
1. Crea un repositorio (recomendado **privado**) y sube estos ficheros.
2. En Netlify: **Add new site → Import an existing project → GitHub**, elige el repo.
   - Build command: *(vacío)* · Publish directory: `.`
3. Cada `git push` vuelve a desplegar solo.

> **Nota de privacidad:** `profesorado/` es accesible por URL si alguien la adivina. Para restringirla: contraseña de sitio en Netlify (plan de pago) o publicar el profesorado en un sitio/repo aparte no enlazado.
