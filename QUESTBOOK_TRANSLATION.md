# 123Technology English Questbook

This fork includes English text for the existing Better Questing chapter and all 31 machine quests. The translation was merged from [pull request #1](https://github.com/leeshea89-collab/123Technology/pull/1).

## What has changed

Only the `name:8` and `desc:8` fields in 32 Better Questing JSON files have been translated. Quest IDs, objectives, machine requirements, prerequisites, rewards, and Java code have not been changed.

The mod's existing `QuestLoader` copies bundled quests into `config/betterquesting/DefaultQuests` at game startup, so the translated text is included in the compiled mod rather than requiring users to run an external script.

## Getting the compiled JAR

1. Open the fork's [GitHub Actions](https://github.com/leeshea89-collab/123Technology/actions) page.
2. Select the latest **Build and test** run on `main` and wait for it to complete successfully.
3. Download the `build-libs` artifact (or an individual JAR artifact if provided).
4. Extract it if necessary, then install the compiled mod JAR in your GTNH `mods` folder, replacing the older version of the same mod. Do not keep both copies.
5. Back up your GTNH instance and quest data first. Restart the game for `QuestLoader` to copy the translated quests.

For an existing world, refreshing Better Questing's default quests may be necessary; back up quest data before running an administrative reload command.

This documentation commit also starts a fresh build on `main` after GitHub Actions was enabled for the fork.
