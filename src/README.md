# grammY Emoji

Adds emoji parsing for [grammY](https://github.com/grammyjs/grammY). Check out the [official documentation](https://grammy.dev/plugins/emoji.html) to learn more about this plugin.

## Installation

```ts
import {...} from "https://github.com/grammyjs/emoji/src/mod.ts";
```

## Example Usage

```ts
bot.command("ping", async (ctx) => {
    // Don't know emoji names? No problem!
    // Press Ctrl + Space on supported editors to
    // see IntelliSense auto-completion magic.
    await ctx.reply(ctx.emoji`Pong! ${"ping_pong"}`);
    // > Pong! 🏓
});

bot.command("start", async (ctx) => {
    await ctx.replyWithEmoji`Welcome to my bot! ${"grinning_face_with_big_eyes"}`;
    // > Welcome to my bot! 😀
});
```

## Pull Requests

Contributions are more than welcome! Just make sure if there is already a similar PR, so you can contribute from there.
