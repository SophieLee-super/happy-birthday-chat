# Happy Birthday, in a Chat 🎂 生日快乐，在聊天里

▶ **Live demo: https://sophielee-super.github.io/happy-birthday-chat/**

A tiny interactive birthday website — a programmer's-romance gift for a friend.
One single `index.html`, no build step, no dependencies. Open it and it plays.

一个小小的互动生日网站 —— 送给朋友的「程序员的浪漫」。单个 `index.html`，无需构建、无依赖，打开就能玩。

## 中文 / English — one page, two languages（v7 新增）

- 页面右上角有 **中文 / EN** 切换按钮：整个网站一键切换语言 —— 聊天剧本（包括按生日星期自动生成的「疯狂星期 X」笑话）、生日特别篇的全部文案、蛋糕与信件、所有按钮和提示。
- 默认中文；链接带 `?lang=en` 可直接以英文打开。`?date=` 与 `?lang=` 可以同时使用。
- The **中文 / EN** switch (top-right) flips the whole site between Chinese and English — the chat script (including the auto-computed "Crazy Weekday" joke), every birthday-fact screen, the cake, the letter, and all UI labels. Chinese by default; add `?lang=en` to a link to open it in English. Works together with `?date=`.

> 自 v7 起，本项目的中英文合并在同一个项目、同一个页面里，不再拆分单独的中文版 / 英文版仓库。Since v7, the Chinese and English versions live in this one project and one page — no separate language repos.

## What it does

1. **A simulated chat** — messages arrive one by one in a phone-style chat box, with typing dots and tap-to-reply choices (a small branching script, including a "Crazy Weekday" joke that follows the real weekday of the birthday).
2. **What's special about your birthday** — one plain sentence per screen, tap to see the next: the weekday you were born, who shares your birthday, what happened on this day in history, your birth flower, how many days you've been in the world, and the age you're turning.
3. **Balloons, lights and a cake** — balloons rise from the bottom of the screen, and there's one candle to tap out and make a wish.
4. **A letter** — typed out character by character at the end.

## Make it yours in one minute

Everything personal lives in `CONFIG` blocks at the top of the script inside `index.html` — `CONFIG_ZH` for Chinese and `CONFIG_EN` for English:

- Change `birthDate` to your friend's birthday (`YYYY-MM-DD`) — the weekday joke and the whole "special birthday" section regenerate automatically, in both languages.
- Or just share a link with the date in it: `index.html?date=2007-01-07` — the date in the link wins, no code editing needed. Add `&lang=en` for English.
- Edit the chat lines, the choice replies, and the letter text in the CONFIG blocks, word for word however you like.
- Same-day celebrities / history lines live in small lookup tables keyed by `MM-DD` in each language — add your friend's date if it's not there yet (dates not in the table simply skip those two lines).

## Run it / publish it free

- Locally: just open `index.html` in any browser.
- Online: enable **GitHub Pages** (Settings → Pages → Deploy from branch `main`, folder `/ (root)`) and share the link it gives you. Add `?date=YYYY-MM-DD` to the link to generate the site for that birthday.

## License

MIT — fork it, change the words, and give it to your own person.
