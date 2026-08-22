# simulacro-mtc-web

Landing page de **Simulacro MTC Perú**, la versión peruana (flavor `peru`) de la app
`simulacro-mtc-flutter`.

- Sitio estático de un solo archivo: [`index.html`](index.html). Sin build, sin dependencias.
- Se publica con GitHub Pages en <https://zeytx.github.io/simulacro-mtc-web/>.
- `app-ads.txt` autoriza el publisher de AdMob (`pub-3426154531596547`).

## Assets

| Archivo | Origen |
|---|---|
| `assets/app-icon.png`, `apple-touch-icon.png`, `favicon.png` | `AppIconPeru.appiconset/Icon-App-1024x1024@1x.png` de la app |
| `assets/ec-icon.png` | `AppIconEcuador.appiconset` (enlace cruzado a la web de Ecuador) |
| `assets/og-image.png` | generado a partir del icono |
| `assets/qr-code.png` | QR a la ficha del App Store |

`qr-code.png` en la raíz es el QR de la versión anterior del sitio y ya no se usa.

## Datos que muestra la página

Salen del pack de país `lib/countries/peru/peru_config.dart` y de `assets/` en el repo de la app.
Si cambian allí, actualizar aquí:

- Examen: **40 preguntas / 40 minutos / 35 aciertos** para aprobar.
- Banco: **2 178 preguntas** (407 con imagen), **16 temas**.
- Categorías: `A1`, `A2a`, `A2b`, `A3a`, `A3b`, `A3c`, `B2a`, `B2b`, `B2c`
  (`A1` viene desbloqueada, `A3c` es solo Premium).
- App Store ID: `6756247516` · Bundle: `com.altech.simulacromtc`.

La web hermana de Ecuador vive en [`simulacro-anc-web`](https://github.com/zeytx/simulacro-anc-web)
y comparte el mismo sistema visual con la paleta amarilla/azul del flavor `ecuador`.
