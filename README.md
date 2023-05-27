# Palettey
🎨 Palettey is a Discord bot for generating color palettes based on an input color. It was created by Tadeas Jun in 2023. The bot allows Discord user to generate color palettes
of 3 - 21 colors relevant to an input color. The bot is fully written in PHP using the DiscordPHP library.

## Invite the bot
The Palettey Bot is hosted 24/7 by the author, and is available for anyone to use freely. You can invite the bot to your server(s) using [this link](https://discord.com/oauth2/authorize?client_id=1111650904563798017&permissions=0&scope=bot%20applications.commands).

## Accepted color formats
Each commands takes a required argument of the color the palette should be generated around. Accepted formats are:
- hexcode (`#ff652f`)
- shorthand hexcode (`#f60`)
- RGB values (`rgb(255, 120, 0)`)

More color formats can be added per suggestions.

## Palette-generating algorithms
The bot currently uses two algorithms to generate the color palettes, both available as separate commands.

The Darken-Ligten algorithm places the input color in the middle of the palette and generates darker / lighter colors around it by subtracting / adding a constant value to each of the RGB values.
The first example palette was generated using this algorithm and the input color `#2d2c2c`.

The Contrasting Color algorithm fills up most of its palette using the Darken-Lighten algorithm, but the last two colors of the palette are dedicated to a contrasting color and its darker version.
The contrasting color is found by finding the opposite side of the color wheel - i.e. calculating the `255 - x` value for each of the RGB values.
The second and third example palettes were generated using this algorithm and the input colors `#ff652f` and `#516868`.

## Contact
If you have any questions about Palettey, if you need an PHP / Discord developer, or if you just want to chat for a while, please feel free to reach out to Tadeas using his email contact@tadeasjun.com, or on Discord - **Tadeas Salvatore Jun#9537**.
