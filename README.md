# Panel de patrimonio (versión gratuita)

Herramienta para ver tu patrimonio en un solo sitio y preparar los datos de la declaración de la Renta a partir de tus propios CSV/Excel. Funciona en local: tus datos no salen de tu ordenador.

> **Aviso importante:** esto es una herramienta de cálculo. No es asesoramiento financiero ni fiscal, ni una recomendación de inversión. Las cifras son orientativas: revísalas siempre con tu gestor o asesor fiscal antes de presentar nada a Hacienda.

## Descarga

Tienes dos formas. Elige la que te dé más tranquilidad.

### Opción 1 (la más sencilla y transparente): el archivo HTML

- Archivo: [`Panel-de-patrimonio-Normal.html`](Panel-de-patrimonio-Normal.html) (unos 780 KB).
- Pulsa en el archivo y luego en el botón de descarga (flecha hacia abajo), o usa «Download raw file».
- Haz doble clic en el archivo descargado: se abre en tu navegador. No hay que instalar nada ni ejecutar ningún programa.
- Es un único archivo de texto: si quieres, puedes abrirlo con el Bloc de notas y ver qué contiene. Funciona sin conexión y no envía tus datos a ningún sitio.
- Qué no tiene: la consulta automática de precios, que necesita el programa de la opción 2. Puedes anotar los precios a mano.

### Opción 2: programa para Windows o Mac (con precios automáticos)

Ve a la sección **Releases** (columna derecha de esta página) y descarga la última versión para tu sistema:

- Windows: `Panel-de-patrimonio-Normal-Windows.zip`
- Mac: `Panel-de-patrimonio-Normal-Mac.zip`

Descomprime y abre. Dentro hay un `LEEME.txt` con los pasos.

**Si Windows muestra «Windows protegió su PC»:** es normal en programas de editores poco conocidos; Windows avisa por reputación, no porque haya detectado un problema. Si quieres continuar, pulsa **Más información** y luego **Ejecutar de todas formas**. Si prefieres no ejecutar nada, usa la opción 1.

## ¿Cómo sé que el archivo es el original? (opcional)

Cada archivo tiene una «huella» (SHA-256): una cadena larga de letras y números que cambia por completo si el archivo se modifica aunque sea en una coma. Si la huella de tu descarga coincide con la de esta tabla, el archivo es idéntico al que yo publiqué.

En Windows, abre PowerShell en la carpeta de descarga y escribe (cambia el nombre por el del archivo):

```
Get-FileHash .\Panel-de-patrimonio-Normal.html -Algorithm SHA256
```

En Mac, abre Terminal en esa carpeta y escribe:

```
shasum -a 256 Panel-de-patrimonio-Normal.html
```

Compara el resultado con esta tabla (versión 6.28):

| Archivo | Huella SHA-256 |
|---|---|
| `Panel-de-patrimonio-Normal.html` | `15c4d759eeb0575422b8f38553f678e3fabf8d0296673ce10b62356458b07cf7` |
| `Panel-de-patrimonio-Normal-Windows.zip` | `38a20a176bd3d2e643c5f5c8314770086fc5b542f7ef652669074f9ece0a7620` |
| `Panel-de-patrimonio-Normal-Mac.zip` | `2cc931b7f2a7df6397d43d8cd329a4ec8903e6ac743003634d7b3014611ae0fc` |

Si no coincide, no lo uses.

## Qué incluye la versión gratuita

- **Inicio y Cartera:** visión global de tu patrimonio.
- **Operaciones:** importa CSV/Excel o añade operaciones a mano.
- **Calidad de datos:** avisa de operaciones raras, duplicadas o incompletas.
- **Rendimiento:** rentabilidad TWR y TIR.
- **Objetivos:** simulación de Montecarlo.
- **Fiscalidad:** resumen por ejercicio, aviso del umbral de los modelos 720/721, ajustes y reglas, y el total anual para la Renta.

Plataformas que puede importar: Trade Republic, Bit2Me, Bitvavo y extractos bancarios en CSV/Excel (por ejemplo, Banco Santander). ¿Usas otra? Cuéntamelo (ver «Feedback»).

## Antes de usarla

- Es una versión en pruebas: puede tener errores.
- Trabaja siempre con copias de tus CSV/Excel, no con los originales.
- No guardes ni compartas contraseñas ni claves de acceso en la herramienta.

## Feedback

Busco opiniones sinceras: qué te falta, qué te confunde y qué plataformas te interesaría importar.

- Abre un **issue** en este repositorio y me cuentas.
- Si me envías un CSV de una plataforma que aún no está soportada, **anonimízalo antes**: borra nombre, IBAN, DNI y cualquier dato que te identifique, y cambia importes y fechas si quieres. Lo usaré solo para crear el importador y lo eliminaré después.

## Condiciones de uso

Uso gratuito y personal. No se permite redistribuir los archivos ni venderlos. El software se ofrece «tal cual», sin garantías; el autor no se hace responsable de decisiones tomadas a partir de sus resultados.

Autor: iasgg86
