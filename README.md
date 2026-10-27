# The Body Clock Mandala

The Traditional Chinese Medicine body clock in one circle. A single static page (`index.html`), no build step.

The wheel is a 24-hour clock with noon at the top and midnight at the bottom. From the center out:

- **Qi, yin and yang**: the yin-yang symbol, drawn so its bright head sits at noon and its dark head at midnight.
- **The Five Phases** (Wu Xing): six arcs over the clock (Metal, Earth, Fire, Water, Fire, Wood). Fire has two: sovereign (Heart, Small Intestine) and ministerial (Pericardium, Triple Burner).
- **The twelve organ hours**, two hours each, Lung at 3 am round to Liver at 1 am, each with its yin or yang marked in the panel.
- **In daily life** petals, then a narrow band with each organ's **feeling or quality**.
- **The four seasons of the day** (Ling Shu 44): spring at dawn (3 to 9 am), summer at midday, autumn at dusk, winter at night, with four small **Earth** markers at the hinges (3 am, 9 am, 3 pm, 9 pm).
- An outer ring of 24 hour petals, with noon gold and midnight indigo.

Tabs: How to read, Qi, Five Phases (with the generating and controlling cycles), Metal, Earth, Fire, Water, Wood (each with its organ cards), Seasons of the day, Practice.

## Editing

All content is in the `RINGS`, `ELEMENTS`, `ORGANS`, `ELARCS`, `SEASONS`, `HINGES`, `QI`, `PRACTICE`, and `FIVE` objects near the top of the script. Ring radii are in `R`. Light and dark mode is saved as `tcm-theme`.

Preview with the `tcm-mandala` entry in DreamWave's `.claude/launch.json`, or `python3 -m http.server --directory .`.

## Live

Published with GitHub Pages from `main` at https://erinsarita.github.io/tcm-mandala/. A push updates the live site.

## Not yet done

Not on the Living Mandalas hub. To add it there: save light and dark 800 × 800 images of the wheel to the hub's `img/`, then add a `MANDALAS` entry with `themeKey: "tcm-theme"`.
