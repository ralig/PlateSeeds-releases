# PlateSeeds

Plan PlateUp speedrun seeds: find seeds whose cards fit what you want, see every shop and reroll along the way, and plan the blueprints you need day by day.

PlateSeeds assumes the **"Seeds affect everything"** game option, so the cards, shops and rerolls it shows are the ones that seed will give you.

## Download

Get the latest **PlateSeeds.App-win-Setup.exe** from [Releases](../../releases/latest) and run it.

- It installs for your Windows user only (no admin), adds a Start menu shortcut, and installs Microsoft's .NET 9 Desktop Runtime if you don't have it.
- Windows may say *"Windows protected your PC"* because the app isn't signed: click **More info**, then **Run anyway**.
- Rather not install? The **Portable.zip** on the same page runs from any folder (it needs the .NET 9 Desktop Runtime).

## Requirements

- Windows 10 or 11, 64-bit
- PlateUp installed through Steam (PlateSeeds reads the game's cards, dishes and blueprints from your copy; it doesn't ship any of the game's data)

## First run

PlateSeeds finds PlateUp in your Steam libraries and reads its data (a few seconds). If it can't find it, paste the folder that holds PlateUp.exe (in Steam: PlateUp, Manage, Browse local files).

## After a PlateUp update

Open **Settings** (the ⚙ at the top right) and press **Update game data**. That covers new cards, dishes and blueprints. If an update changes how shops or rerolls work, PlateSeeds will be wrong until it's updated too.

## What's in it

- **Search:** seeds whose card path fits a query: cards on each day, layouts, the front door, fewer customers, blueprints a shop offers by a day.
- **Card tree:** a seed's cards day by day, and its starting restaurant.
- **Blueprints:** every shop and reroll along the path, a day-by-day plan with coins estimated, and the way to any blueprint you highlight.
- **Wish list:** list the blueprints you want and let it plan them onto the run.
- **Compare:** plan several seeds side by side.
- **Plan overview:** the whole plan in its own window to keep beside the game, with a live page you can share.

What changed in each version: [CHANGELOG.md](CHANGELOG.md), also in the app (Settings, About, Changelog).

## Live sharing

The plan overview can share your plan live as a web page anyone with the link can follow. It stores the plan in a secret GitHub Gist, so it needs a GitHub account and a token with the *gist* permission (Settings, Live plan sharing, Create a token). A secret gist is unlisted, not private: anyone with the link can read it.

## Command line

`plateseeds-cli.exe` sits beside the app, for automating searches and the rest. Run `plateseeds-cli --help` for the commands; `plateseeds-cli update-data` reads the game data without opening the app.

## Uninstall

Windows Settings, Apps, PlateSeeds. Your settings and the game data it read stay in `%LOCALAPPDATA%\PlateSeeds`; delete that folder to remove them too.

## Privacy

PlateSeeds sends nothing anywhere, except the plans you choose to share live (to your own GitHub Gist).

## Credits

Vibe coded with Claude. MIT licensed; see [LICENSE](LICENSE) and [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt). PlateUp is by It's Happening; PlateSeeds is a fan tool, not made or endorsed by them.
