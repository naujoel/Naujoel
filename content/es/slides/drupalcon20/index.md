---
title: Diapositivas
summary: DrupalCon une a diversos expertos de todo el mundo que crean experiencias digitales ambiciosas.
authors: []
tags: []
categories: []
date: ""
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: black
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: dracula
---

# Bienvenido a Minneapolis

[Drupal](https://drupal.org/) | [DrupalCon Minneapolis 2020](https://events.drupal.org/minneapolis2020)

---

## Caracteristicas

- En Minneapolis, nunca estás a más de seis manzanas de un parque, y es probable que también veas algunos lagos.
- Minneapolis es el hogar de una próspera cultura de comida, música y actividades al aire libre.
- Desde el Puente Stone Arch hasta las Cataratas Minnehaha, desde el Distrito de las Artes del Nordeste hasta Eat Street, hay una joya de ciudad por descubrir.
- Descubrir es parte de DrupalCon, así que planea unirte a nosotros en Minneapolis.

---

## Hazte patrocinador

- DrupalCon Norteamérica es consistentemente el evento Drupal con mayor asistencia en el mundo.
- En 2020, presentaremos un calendario completo de oportunidades educativas, de redes y de contribución.
- La creciente comunidad adquirirá nuevas habilidades y celebrará a medida que avancemos en el proyecto Drupal.
- Patrocinar a DrupalCon puede ayudar a su negocio con el conocimiento de la marca, el reclutamiento de talentos, la creación de redes con socios y clientes potenciales, la generación de clientes potenciales, el apoyo de la comunidad y el liderazgo intelectual.

---

## Code Highlighting

Inline code: `variable`

Code block:
```python
porridge = "blueberry"
if porridge == "blueberry":
    print("Eating...")
```

---

## Math

In-line math: $x + y = z$

Block math:

$$
f\left( x \right) = \;\frac{{2\left( {x + 4} \right)\left( {x - 4} \right)}}{{\left( {x + 4} \right)\left( {x + 1} \right)}}
$$

---

## Fragments

Make content appear incrementally

```
{{%/* fragment */%}} One {{%/* /fragment */%}}
{{%/* fragment */%}} **Two** {{%/* /fragment */%}}
{{%/* fragment */%}} Three {{%/* /fragment */%}}
```

Press `Space` to play!

{{% fragment %}} One {{% /fragment %}}
{{% fragment %}} **Two** {{% /fragment %}}
{{% fragment %}} Three {{% /fragment %}}

---

A fragment can accept two optional parameters:

- `class`: use a custom style (requires definition in custom CSS)
- `weight`: sets the order in which a fragment appears

---

## Speaker Notes

Add speaker notes to your presentation

```markdown
{{%/* speaker_note */%}}
- Only the speaker can read these notes
- Press `S` key to view
{{%/* /speaker_note */%}}
```

Press the `S` key to view the speaker notes!

{{< speaker_note >}}
- Only the speaker can read these notes
- Press `S` key to view
{{< /speaker_note >}}

---

## Themes

- black: Black background, white text, blue links (default)
- white: White background, black text, blue links
- league: Gray background, white text, blue links
- beige: Beige background, dark text, brown links
- sky: Blue background, thin dark text, blue links

---

- night: Black background, thick white text, orange links
- serif: Cappuccino background, gray text, brown links
- simple: White background, black text, blue links
- solarized: Cream-colored background, dark green text, blue links

---

{{< slide background-image="/img/boards.jpg" >}}

## Custom Slide

Customize the slide style and background

```markdown
{{</* slide background-image="/img/boards.jpg" */>}}
{{</* slide background-color="#0000FF" */>}}
{{</* slide class="my-style" */>}}
```

---

## Custom CSS Example

Let's make headers navy colored.

Create `assets/css/reveal_custom.css` with:

```css
.reveal section h1,
.reveal section h2,
.reveal section h3 {
  color: navy;
}
```

---

# Questions?

[Ask](https://spectrum.chat/academic)

[Documentation](https://sourcethemes.com/academic/docs/managing-content/#create-slides)
