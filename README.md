# ISW_4K1_G1_2026

## Estructura del Repositorio

```
ISW_4K1_G1_2026
├── README.md
├── material_catedra
│       ├── bibliografia
│       ├── clases_grabadas
│       ├── consignas_tps
│       │       ├── tps_evaluables
│       │       ├── tps_no_evaluables
│       │       └── trabajos_investigacion
│       ├── planificacion
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
                ├── tps_no_evaluables
                └── trabajos_investigacion
```

## Ítems de Configuración

| Tipo de Ítem | Ítem de Configuración | Regla de Nombrado | Ubicación Física | Formatos |
|---|---|---|---|---|
| producción_propia | Ejercicios | `ejercicio-<Titulo_Tema>-<autor>.<ext>` | `produccion_propia/ejercicios/` | .pdf |
| material_clase | Toma de Notas/Apuntes | `apunte-<ddmm>-<ApellidoAutor_NombreAutor>.<ext>` | `material_clase/apuntes/` | .md, .pdf |
| producción_propia | Resumen | `resumen-u<numero_unidad>-<tema>-<ApellidoAutor_NombreAutor>.<ext>` | `produccion_propia/resumenes/` | .pdf |
| material_catedra | Bibliografía | `<Nombre-Archivo>.pdf` | `material_catedra/bibliografia/` | .pdf, .docx |
| material_catedra | Templates | `template-<Titulo_Tema>-<ext>` | `material_catedra/templates/` | .pdf, .docx, .xlsx |
| material_catedra | Diapositiva de Clase | `diapositiva-<numero>-<Titulo_Tema>.pdf` | `material_catedra/presentaciones_de_clase/` | .pdf |
| material_catedra | Consigna TP Evaluable | `consigna-tp-<numero>.pdf` | `material_catedra/consignas_tps/tps_evaluables/` | .pdf |
| producción_propia | Entrega TP Evaluable | `entrega-tp-<numero>-<Titulo_Tp>.<ext>` | `produccion_propia/trabajos_practicos/tps_evaluables/` | .pdf, .zip |
| material_catedra | Consigna TP No Evaluable | `consigna-tp-<numero>.pdf` | `material_catedra/consignas_tps/tps_no_evaluables/` | .pdf |
| producción_propia | Entrega TP No Evaluable | `entrega-tp-<numero>-<Titulo_Tp>.pdf` | `produccion_propia/trabajos_practicos/tps_no_evaluables/` | .pdf |
| material_catedra | Consigna Trabajo de Investigación | `consigna-ti-<numero>-<Titulo_Ti>.pdf` | `material_catedra/consignas_tps/trabajos_investigacion/` | .pdf |
| producción_propia | Entrega Trabajo de Investigación | `entrega-ti-<numero>.<ext>` | `produccion_propia/trabajos_practicos/trabajos_investigacion/` | .pdf, .png |
| material_catedra | Cronograma | `cronograma-isw.xlsx` | `material_catedra/planificacion/` | .xlsx |
| material_catedra | Programa | `programa-isw.pdf` | `material_catedra/planificacion/` | .pdf |

## Aclaraciones sobre Entregas

> **TP06:** Además del `.pdf`, se debe subir el código fuente comprimido en un archivo `.zip`.


## Reglas de Nombrado

- **Carpetas:** Absolutamente todas las carpetas utilizarán el formato `snake_case` (ej. `trabajos_practicos`). No se admiten acentos, eñes, ni mayúsculas.
- **Archivos:** Absolutamente todos los archivos utilizarán el formato `kebab-case` (ej. `consigna-tp-01.pdf`). No se utilizará el versionado en el nombre del archivo (nunca `tp-01-v2.pdf` ni `tp-01-final.pdf`); el control de versiones lo delega exclusivamente el SCM (Git). Los títulos de presentaciones, tps, etc serán definidos por el formato Pascal Snake Case o también conocido como Ada_Case.
- **Tags (Líneas Base):** Se utilizará el formato `lb-<tipo>-<identificador>`. El prefijo `lb-` indicará siempre que el tag representa una Línea Base. Ejemplos: `lb-tp-01` (para el TP Evaluable 1), `lb-ti-01` (para el Trabajo de Investigación 1), `lb-parcial-01` (para los apuntes y resúmenes consolidados del primer parcial).

## Criterio de Línea Base

Una Línea Base se establece ante toda instancia de evaluación formal que haya recibido devolución con nota por parte de la cátedra, una vez que los ICs involucrados cumplan los siguientes criterios:

1. Revisado y aprobado por al menos un integrante distinto al autor (Peer Review).
2. Completo y en versión definitiva, con correcciones incorporadas y sin marcas de borrador.
3. Respeta el formato y la ubicación definidos en la matriz de ICs.
4. No hay trabajo en progreso sobre ninguno de los ICs incluidos.

Una Línea Base no implica modificar los nombres de los archivos. En su lugar, se materializa técnicamente en el repositorio mediante el uso de **Git Tags anotados**.

## Glosario

| Variable | Descripción |
|---|---|
| `<tema>` | Palabra clave descriptiva del contenido en minúsculas y sin espacios (ej. `requerimientos`, `patrones`, `scrum`). |
| `<ApellidoAutor_NombreAutor>` | Primer apellido del autor en con inicial en mayúsculas (ej. Pérez) seguido del nombre del autor con la inicial en mayúsculas. Si el documento es grupal, se omitirá esta variable o se usará `grupo1`. |
| `<ext>` | Extensión del archivo explícitamente permitida en la tabla de ICs (ej. `pdf`, `md`). |
| `<ddmm>` | Fecha de la clase o nota, expresada en 4 dígitos numéricos (ej. `2408` para el 24 de agosto). |
| `<numero_unidad>` | Número de la unidad temática con dos dígitos (ej. `01`, `04`). |
| `<numero>` | Identificador numérico correlativo con un cero a la izquierda para mantener el orden alfabético en el explorador (ej. `01`, `02`, `03`). |
| `<Titulo_Tp/Ti>` | Nombre del trabajo práctico/de investigación a entregar. |
| `<Nombre-Archivo>` | Nombre original del archivo provisto por la cátedra, con las iniciales en mayúsculas y separado por guiones (ej. `Sommerville-Cap-4`). |
| `<tipo>` | Clasificación del hito que da origen a la Línea Base, siempre en minúsculas. Valores permitidos: `tp` (Trabajo Práctico Evaluable), `ti` (Trabajo de Investigación), o `parcial` (Evaluación Parcial). |
| `<identificador>` | Número o texto breve que identifica unívocamente al hito dentro de su tipo. Para TPs y TIs debe coincidir con el `<numero>` (ej. `01`, `02`). Para parciales puede ser el número o instancia (ej. `01`, `02`, `01-recuperatorio`). |

## Link al Repositorio

[https://github.com/Pablo-Ramos-M/ISW_4K1_G1_2026.git](https://github.com/Pablo-Ramos-M/ISW_4K1_G1_2026.git)
