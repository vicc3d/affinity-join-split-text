# Join & Split Text for Affinity

Split a paragraph into one text object per line, or join several text objects into one
paragraph, in [Affinity](https://www.affinity.studio/) (v3, by Canva). The UI comes in English
and Spanish.

## Features

- **Split** the selected texts:
  - **by line**: every line as you see it, including the lines a text frame wraps on its own;
  - **by paragraph**.
  - Each new text keeps its character formatting (font, size, colour, tracking…) and lands
    exactly where the line was.
  - Output: the same type as the original, artistic text, or text frames.
- **Join** the selected texts into one:
  - reading order, top to bottom or left to right;
  - separator: space, line break, paragraph break, or nothing;
  - also joins the lines inside each text (optional), so one text with manual line breaks
    becomes a single paragraph;
  - rejoins words split with a hyphen at the end of a line (`lí-` + `nea` → `línea`);
  - keeps each piece's formatting (optional).
- Works with **artistic text** and **text frames**, also inside groups.
- **One Ctrl+Z** undoes everything. Optionally keeps the original objects.

## Install

1. Download [`text-joiner.en.js`](text-joiner.en.js) (English UI) or
   [`text-joiner.es.js`](text-joiner.es.js) (Spanish UI).
2. Install it through [Affinity Script Manager](https://github.com/JiriKrblich/Affinity-script-manager),
   or create a new script in Affinity's Scripts panel and paste the code.

## Use

1. Select one or more texts.
2. Run **Join & Split Text** (Spanish build: **Unir y separar texto**).
3. Choose **Split** or **Join** and the options, then press **OK**.

With a single text selected, the dialog opens in Split mode; with several, in Join mode.

## Limitations

- Rotated, skewed or flipped texts and linked text frames are skipped.
- Splitting by line in a frame breaks at word ends. A word that is hyphenated by automatic
  hyphenation, or is too long for the frame, stays whole on one line.
- Split lines are rebuilt from their character formatting. Object-level settings of the
  original (layer effects, opacity) are not copied.
- Justified lines come out left-aligned when split (each one is the last line of its paragraph).
- Joining into a text frame doesn't resize it; enlarge the frame if the text overflows.
- Fields (page numbers, data merge…) become plain text when joined or split.

## License

[MIT](LICENSE)

---

## Español

Separa un párrafo en un texto por línea, o une varios textos en un solo párrafo.

- **Separar** por **líneas** (tal como se ven, incluidas las que el marco corta solo) o por
  **párrafos**. Cada texto nuevo conserva el formato y queda exactamente donde estaba la línea.
- **Unir** en orden de lectura, con espacio, salto de línea, salto de párrafo o nada; une
  palabras cortadas con guion y conserva el formato de cada fragmento.
- Texto artístico y marcos de texto, también dentro de grupos. **Un solo Ctrl+Z** lo deshace.

Instalación: descarga [`text-joiner.es.js`](text-joiner.es.js) e instálalo con Affinity Script
Manager, o crea un script nuevo en el panel Scripts de Affinity y pega el código.
