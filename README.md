# radar-tendencias-aimax

Skill para **Claude Code** que busca tendencias e ideas de contenido de tu nicho en tiempo real (con búsqueda web) y te devuelve una lista de ideas listas para grabar: hook + ángulo + formato + por qué ahora + fuente.

No necesita ningún conector de Instagram. Es la pieza que te dice **qué publicar a continuación** — complementaria a los MCP de Instagram (Metricool, Composio), que te dicen cómo rinde lo que ya publicaste.

Creada por [@david_ai_pro](https://instagram.com/david_ai_pro) para la comunidad **AIMAX Labs**.

---

## Qué hace

- Coge tu sector y hace un barrido de búsquedas por 6 ángulos (tendencia actual, formatos que funcionan, noticias, dolores de la audiencia, competencia, estacionalidad).
- Destila 7-10 ideas de contenido actuales, cada una con su fuente.
- Marca el "tema caliente de la semana".
- No se inventa nada: todo lo que propone se apoya en una búsqueda reciente.

---

## Instalación (déjasela a Claude Code)

No tienes que descargar ni descomprimir nada a mano. Abre Claude Code y pégale uno de estos dos prompts, según dónde quieras usar la skill.

### Opción A · Global (en todos tus proyectos)

Queda disponible en cualquier proyecto que abras con Claude Code. Es lo recomendable si vas a buscar tendencias a menudo.

```
Instala una skill desde GitHub. Descarga este repositorio:
https://github.com/david-ai-pro/radar-tendencias-aimax
Dentro hay una carpeta radar-tendencias-aimax con su SKILL.md: instálala como skill GLOBAL
copiando esa carpeta entera en la carpeta de skills globales de Claude Code
(~/.claude/skills/ — en Windows es C:\Users\MI_USUARIO\.claude\skills\).
Si la carpeta skills no existe, créala. Cuando acabes, confírmame la ruta exacta
donde ha quedado y qué hace la skill.
```

### Opción B · Solo en el proyecto abierto

La instala únicamente dentro de la carpeta del proyecto que tengas abierto, sin tocar el resto. Ideal si solo la quieres para un proyecto concreto.

```
Instala una skill desde GitHub SOLO en este proyecto (no en global). Descarga este repositorio:
https://github.com/david-ai-pro/radar-tendencias-aimax
Dentro hay una carpeta radar-tendencias-aimax con su SKILL.md: instálala como skill DE PROYECTO
copiando esa carpeta entera dentro de la carpeta de skills del proyecto actual
(.claude/skills/ en la raíz de este proyecto).
Si la carpeta .claude/skills no existe, créala. Cuando acabes, confírmame la ruta exacta
dentro del proyecto y qué hace la skill.
```

Reinicia Claude Code (las skills se cargan al arrancar) y comprueba:

```
¿Tienes disponible la skill radar-tendencias-aimax? Explícame en dos frases qué hace.
```

---

## Cómo usarla

```
Busca tendencias e ideas de contenido de esta semana para mi nicho.
```

La primera vez te preguntará tu sector, plataforma y público. Puedes guardarlo en un archivo `mi-nicho.md` (la skill se ofrece a crearlo) para no repetirlo cada vez.

También responde a: "qué contenido hago esta semana", "qué está petando en [tu nicho]", "ideas para reels de [tema]", o directamente `/radar-tendencias`.

---

## Convertirlo en rutina automática (opcional)

Si prefieres que se ejecute solo cada día o cada semana en vez de escribirle tú, pégale a **Claude Code** este prompt y él te montará la rutina, preguntándote antes tu sector, la frecuencia y la hora:

```
Quiero una rutina automática que ejecute la skill radar-tendencias-aimax por mí,
sin que yo tenga que escribirte cada vez. Antes de crearla, pregúntame:
1) mi nicho/sector y mi público, 2) si la quiero diaria o semanal y a qué hora
(y qué día, si es semanal), 3) dónde quiero que me deje el resultado
(un archivo markdown con fecha en una carpeta, o que me lo notifique).
Con esas respuestas, crea la tarea programada usando el sistema de tareas
programadas de Claude Code, deja la skill lista para correr en automático,
y confírmame cuándo se ejecutará la próxima vez y cómo pararla o cambiarla.
```

---

## Contenido del repo

```
radar-tendencias-aimax/              # raíz del repositorio
├─ README.md                         # este archivo
└─ radar-tendencias-aimax/           # la carpeta de la skill (esto es lo que se instala)
   ├─ SKILL.md                       # la skill (instrucciones para Claude)
   └─ references/
      ├─ playbook-busqueda.md        # las búsquedas por ángulo, ampliadas
      └─ mi-nicho-plantilla.md       # plantilla de configuración de nicho
```

## Licencia

MIT. Úsala, modifícala y compártela.
