# Illustrated ad · omnigami

Your ingredients, drawn as we watch.

A 16-second ad for a physical product range. Each product’s ingredients draw themselves stroke by stroke in your packaging’s own illustration style, and the real product rises in front of them, one page after another, ending on all of them together with your line and call to action.

Watch it play live, and change its words, at [omnigami.ai/skills/illustrated-ad](https://omnigami.ai/skills/illustrated-ad).

## Install

In Claude Code:

```
/plugin marketplace add omnigami-ai/skills
/plugin install omnigami-illustrated-ad@omnigami
```

With the skills CLI, for Claude Code and other agents that read SKILL.md:

```bash
npx skills add omnigami-ai/illustrated-ad
```

Or copy `skills/illustrated-ad/` into your agent's skills folder (for Claude Code, `~/.claude/skills/illustrated-ad/`). Then ask:

```
Make an illustrated ad for my three teas: https://your-shop.com
```

## What it runs

The skill works on your computer. It runs the Node scripts in `skills/illustrated-ad/scripts/`: they open your product's pages in a local headless browser to capture its real screens, then render the film with that browser and ffmpeg, writing MP4s and an editable HTML film to your project. It sends nothing to omnigami or anyone else, and uses no network beyond loading your own product's pages and the fonts and assets in this folder.

## You need

- Claude Code with Opus 5.5
- Node 20 or later
- Python 3 with Pillow and NumPy
- ffmpeg
- Chrome, Chromium, Edge or Brave
- An image model for the illustrations (your agent’s own, if it has one)

None beyond your Claude plan’s usage, unless your image model charges for the illustrations.

## Licence

Free to use. Use the films and anything else the skill makes for anything, commercial work included. Don't redistribute the skill. See [LICENSE.md](LICENSE.md). The bundled fonts keep their own licence (SIL Open Font License, beside them in `reference/assets/fonts/`).

## Credits

Its motion is omnigami’s own. Its example shows Fennick, a fictional company made for omnigami’s examples, with sample data.

omnigami is not affiliated with Anthropic. More skills at [omnigami.ai](https://omnigami.ai).
