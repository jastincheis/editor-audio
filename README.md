# Editor Audio

Un editor audio simplu, în stilul Sound Forge, care rulează în browser. E un singur fișier HTML, fără instalare și fără server.

**Deschide-l direct în browser:** https://jastincheis.github.io/editor-audio/

## Ce face

- Deschide **MP3, WAV, FLAC, OGG, M4A**, din buton sau prin drag & drop pe o pistă
- Mai multe piste, fiecare cu forma de undă vizibilă
- **Space** pentru play/pauză, **Esc** pentru stop
- Lipești clipurile cap la cap: se prind magnetic la îmbinare (**Alt** = fără magnet)
- Le suprapui pe piste diferite, cu **volum separat** pentru fiecare clip (−40 … +12 dB)
- **Fade in / fade out** cu mânerele din colțurile clipului sau din câmpurile numerice
- Tai capetele clipului (trăgând de margini), îl tai în două la cursor (**S**), îl ștergi (**Del**), anulezi (**Ctrl+Z**)
- Buton **Mut** pe fiecare pistă
- Salvezi mixul ca **WAV** (16-bit) sau **MP3** (128–320 kbps), la 44.1 sau 48 kHz, cu protecție opțională la distorsiune (limitare la −1 dB)

## Cum îl pornești

Cel mai simplu: deschide https://jastincheis.github.io/editor-audio/ în Chrome sau Chromium.

Local: deschide `index.html` în Chrome sau Chromium. Ca aplicație separată:

```sh
chromium --app=file:///cale/catre/editor-audio/index.html
```

Merge și offline: encoderul MP3 e inclus local.

## Taste

| Tastă | Acțiune |
|---|---|
| Space | Play / pauză |
| Esc | Stop (revine unde a pornit) |
| Home / End | Început / sfârșit |
| ← / → | Înapoi / înainte 1 s (cu Shift: 5 s) |
| S | Taie clipul la cursor |
| Del | Șterge clipul selectat |
| Ctrl+Z / Ctrl+Shift+Z | Anulează / refă |
| Ctrl + rotiță | Zoom |
| Shift + rotiță | Derulare orizontală |

## Componente externe

- [lamejs](https://github.com/zhuker/lamejs) 1.2.1 (`lame.min.js`), encoder MP3, licență LGPL-3.0
