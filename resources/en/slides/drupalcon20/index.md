---
title: Slides
summary: DrupalCon unites diverse experts from around the globe who create ambitious digital experiences.
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

# Welcome to Minneapolis

[Drupal](https://drupal.org/) | [DrupalCon Minneapolis 2020](https://events.drupal.org/minneapolis2020)

---

## Features

- In Minneapolis, you're never more than six blocks from a park, and chances are you'll see a few lakes as well.
- Minneapolis is home to a thriving culture of food, music, and the great outdoors.
- From the Stone Arch Bridge to Minnehaha Falls, from Northeast Arts District to Eat Street, there's a gem of a city to be discovered.
- Discovery is part of DrupalCon, so plan to join us in Minneapolis.

---

## Become a sponsor

- DrupalCon North America is consistently the most widely attended Drupal event in the world.  
- In 2020, we’re featuring a full schedule of educational, networking and contribution opportunities.
- The growing community will gain new skills and celebrate as we advance the Drupal project.
- Sponsoring DrupalCon can help your business with brand awareness, talent recruitment, networking with potential partners and customers, lead generation, community support and thought leadership.


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
