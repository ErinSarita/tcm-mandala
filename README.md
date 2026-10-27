# The Body Clock Mandala

The roots of Five Phase theory, the Traditional Chinese Medicine body clock, and the Five Phase year, in three wheels. A single static page (`index.html`), no build step.

Three wheels share the page, switched by a Phases, Day, and Year toggle above the wheel (remembered as `tcm-view`; `#phases`, `#day`, or `#year` in the address opens one). Phases is first and is the default. Both put noon and midsummer at the top. The Day wheel has no seasons; the year lives on the Year wheel.

**The Phases wheel** is Taoist cosmology from the center out, after Zhou Dunyi: Wuji (the boundless mystery) → Taiji (the first movement) → yin and yang → the Five Phases evenly spaced (Fire at the top, then Earth, Metal, Water, Wood clockwise), with the generating cycle (shēng) as arrows around the circle and the controlling cycle (kè) as a dashed star behind the center → correspondences → the motion of each phase → the ten thousand things. Hovering a phase lights its four relationships. It has no clock and no now mark.

**The Day wheel** is a 24-hour clock with noon at the top and midnight at the bottom. From the center out:

- **Qi, yin and yang**: the yin-yang symbol, drawn so its bright head sits at noon and its dark head at midnight.
- **The Five Phases** (Wu Xing): six arcs over the clock (Metal, Earth, Fire, Water, Fire, Wood). Fire has two: sovereign (Heart, Small Intestine) and ministerial (Pericardium, Triple Burner).
- **The twelve organ hours**, two hours each, Lung at 3 am round to Liver at 1 am, each with its yin or yang marked in the panel.
- **In daily life** petals, then, outermost, a band with each organ's **feeling or quality**.
- An outer ring of 24 hour petals, with noon gold and midnight indigo.

**The Year wheel** is the Five Phases in their seasons. From the center out: the yin-yang; the five phases; the organs each holds; twelve solar-month petals named by their two solar terms; the calendar months; and the five seasons with dates (spring Feb 4 to May 5, summer to Jul 7, late summer to Aug 7, autumn to Nov 7, winter to Feb 4). Seasons start at the four "starts" (lì), so each solstice and equinox is mid-season. Late summer is the sixth solar month (Minor Heat to the Start of Autumn); the 18-days-per-season reading of Earth is explained in the panel. A gold mark on the edge shows the current hour or today's date.

Phases tabs: How to read, Wuji, Taiji, Yin and yang, Five Phases, Correspondences (a full table, the five tastes with foods and example herbs, and feelings on the controlling cycle), Generating, Controlling, Out of balance, Ten thousand things, Practice.

Day tabs: How to read, Qi, Five Phases (with the generating and controlling cycles), Metal, Earth, Fire, Water, Wood (each with its organ cards), Practice.

Year tabs: How to read, Qi, Five Phases, Spring, Summer, Late summer, Autumn, Winter, Practice.

## Editing

Phases wheel content is in `RINGS_C`, `WUJI`, `TAIJI`, `YINYANG`, `PHASES`, `GEN` (phase k feeds k+1), `CTL` (phase k tames k+2), `BALANCE`, `WANWU`, `PRACTICE_C`, `CORR` (organs, sense organ, tissue, sound, taste, climate, emotion, organ hours, and more for each phase), `TASTES`, and `HERB_CARE`, with radii in `RC`. Day and Year content is in the `RINGS`, `RINGS_Y`, `YEAR`, `TERMS`, `MONTHS`, `ELEMENTS`, `ORGANS`, `ELARCS`, `QI`, `PRACTICE`, and `FIVE` objects near the top of the script. Ring radii are in `R`. Light and dark mode is saved as `tcm-theme`.

Preview with the `tcm-mandala` entry in DreamWave's `.claude/launch.json`, or `python3 -m http.server --directory .`.

## Live

Published with GitHub Pages from `main` at https://erinsarita.github.io/tcm-mandala/. A push updates the live site.

## Not yet done

Not on the Living Mandalas hub. To add it there: save light and dark 800 × 800 images of the wheel to the hub's `img/`, then add a `MANDALAS` entry with `themeKey: "tcm-theme"`.
