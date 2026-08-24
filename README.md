# ISW_4K1_G1_2026

## Estructura del Repositorio

```
ISW_4K1_G1_2026
├── README.md
├── material_catedra
│       ├── planificacion
│       ├── bibliografia
│       ├── consignas_tps
│       │       ├── tps_evaluables
│       │       └── trabajos_investigacion
│       ├── templates
│       └── presentaciones_de_clase
├── material_clase
│       ├── ejercicios_en_clase
│       └── apuntes
└── produccion_propia
        ├── resumenes
        ├── ejercicios
        └── trabajos_practicos
                ├── tps_evaluables
                └── trabajos_investigacion
```

## Ítems de Configuración

| Tipo de Ítem | Ítem de Configuración | Regla de Nombrado | Ubicación Física | Formatos |
|---|---|---|---|---|
| producción_propia | Ejercicios | `ejercicio-<tema>-<autor>.<ext>` | `produccion_propia/ejercicios/` | .pdf |
| material_clase | Toma de Notas/Apuntes | `apunte-<ddmm>-<autor>.<ext>` | `material_clase/apuntes/` | .md, .pdf |
| producción_propia | Resumen | `resumen-u<numero_unidad>-<autor>.<ext>` | `produccion_propia/resumenes/` | .pdf |
| material_catedra | Bibliografía | `<nombre-archivo>.pdf` | `material_catedra/bibliografia/` | .pdf, .docx |
| material_catedra | Templates | `template-<tema>-<autor>.<ext>` | `material_catedra/templates/` | .pdf, .docx, .xlsx |
| material_catedra | Diapositiva de Clase | `diapositiva-<numero>-<tema>.pdf` | `material_catedra/presentaciones_de_clase/` | .pdf |
| material_catedra | Consigna TP Evaluable | `consigna-tp-<numero>.pdf` | `material_catedra/consignas_tps/tps_evaluables/` | .pdf |
| producción_propia | Entrega TP Evaluable | `entrega-tp-<numero>-<titulo_tp>.<ext>` | `produccion_propia/trabajos_practicos/tps_evaluables/` | .pdf, .png |
| material_catedra | Consigna Trabajo de Investigación | `consigna-ti-<numero>.pdf` | `material_catedra/consignas_tps/trabajos_investigacion/` | .pdf |
| producción_propia | Entrega Trabajo de Investigación | `entrega-ti-<numero>-<titulo_ti>.<ext>` | `produccion_propia/trabajos_practicos/trabajos_investigacion/` | .pdf, .png |
| material_catedra | Cronograma | `cronograma-isw.xlsx` | `material_catedra/planificacion/` | .xlsx |
| material_catedra | Programa | `programa-isw.pdf` | `material_catedra/planificacion/` | .pdf |

## Reglas de Nombrado

- **Carpetas:** Absolutamente todas las carpetas utilizarán el formato `snake_case` (ej. `trabajos_practicos`). No se admiten acentos, eñes, ni mayúsculas.
- **Archivos:** Absolutamente todos los archivos utilizarán el formato `kebab-case` (ej. `consigna-tp-01.pdf`). No se utilizará el versionado en el nombre del archivo (nunca `tp-01-v2.pdf` ni `tp-01-final.pdf`); el control de versiones lo delega exclusivamente el SCM (Git).
- **Tags (Líneas Base):** Se utilizará el formato `lb-<tipo>-<identificador>`. El prefijo `lb-` indicará siempre que el tag representa una Línea Base. Ejemplos: `lb-tp-01` (para el TP Evaluable 1), `lb-ti-01` (para el Trabajo de Investigación 1), `lb-parcial-01` (para los apuntes y resúmenes consolidados del primer parcial).

## Criterio de Línea Base

En nuestro proyecto, definimos el establecimiento de una nueva Línea Base como un hito formal de estabilización del repositorio. Esto ocurrirá ante los siguientes eventos:

- **Entregas Evaluables:** Tras la devolución y corrección de un Trabajo Práctico Evaluable o de Investigación. Se considera consolidada una entrega cuando las correcciones derivadas de la devolución docente han sido incorporadas y el documento se encuentra en estado definitivo.
- **Hitos Académicos:** Luego de cada evaluación parcial, podrá establecerse una Línea Base, siempre que los ICs correspondientes (resúmenes, apuntes) hayan cumplido previamente los criterios de revisión y no haya trabajo en progreso. Esto asegura que represente un estado estable y controlado del material de estudio, y no solo la ocurrencia de una fecha.

Una Línea Base no implica modificar los nombres de los archivos. En su lugar, se materializa técnicamente en el repositorio mediante el uso de **Git Tags anotados**.

Un ítem de configuración se considera listo para integrar la Línea Base cuando:

1. Ha sido revisado y aprobado por al menos un integrante del grupo distinto al autor (Peer Review).
2. Está completo y en su versión definitiva, sin marcas de borrador.
3. Respeta estrictamente el formato y la ubicación definidos en la matriz de ICs.

## Glosario

| Variable | Descripción |
|---|---|
| `<tema>` | Palabra clave descriptiva del contenido en minúsculas y sin espacios (ej. `requerimientos`, `patrones`, `scrum`). |
| `<autor>` | Primer apellido del autor en minúsculas (ej. `perez`). Si el documento es grupal, se omitirá esta variable o se usará `grupo11`. |
| `<ext>` | Extensión del archivo explícitamente permitida en la tabla de ICs (ej. `pdf`, `md`). |
| `<ddmm>` | Fecha de la clase o nota, expresada en 4 dígitos numéricos (ej. `2408` para el 24 de agosto). |
| `<numero_unidad>` | Número de la unidad temática con dos dígitos (ej. `01`, `04`). |
| `<numero>` | Identificador numérico correlativo con un cero a la izquierda para mantener el orden alfabético en el explorador (ej. `01`, `02`, `03`). |
| `<titulo_tp/ti>` | Nombre del trabajo práctico/de investigación a entregar. |
| `<nombre-archivo>` | Nombre original del archivo provisto por la cátedra, normalizado a minúsculas y separado por guiones (ej. `sommerville-cap-4`). |
| `<tipo>` | Clasificación del hito que da origen a la Línea Base, siempre en minúsculas. Valores permitidos: `tp` (Trabajo Práctico Evaluable), `ti` (Trabajo de Investigación), o `parcial` (Evaluación Parcial). |
| `<identificador>` | Número o texto breve que identifica unívocamente al hito dentro de su tipo. Para TPs y TIs debe coincidir con el `<numero>` (ej. `01`, `02`). Para parciales puede ser el número o instancia (ej. `01`, `02`, `01-recuperatorio`). |

## Link al Repositorio

[https://github.com/Pablo-Ramos-M/ISW_4K1_G1_2026.git](https://github.com/Pablo-Ramos-M/ISW_4K1_G1_2026.git)
