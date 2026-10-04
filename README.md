# A Fool's Errand

A warm, silly, Terry Pratchett-lite medieval text adventure, played turn by turn in conversation with Claude.

You are a peasant of no particular distinction, farming something unglamorous, when the Royal Wizard's carriage crashes through your fence. The Wizard, spectacles cracked and hat askew, squints at you and declares you the Chosen One. Your crops are on fire. Gerald, the Wizard's enchanted goose (who actually steers the carriage), is not impressed.

## How to play

Once the plugin is installed, ask Claude:

> Let's play A Fool's Errand.

The game only starts when you ask for it by name, so it won't take over other conversations about games or fantasy.

Each turn, Claude narrates a few sentences and offers three choices (A, B, and C). You can also type anything else you'd like to try. Along the way you'll:

- Keep an eye on your **Gold**, your **Dignity**, and your **Cheese**, which is an extremely important resource in this kingdom
- Work through the three absurd quests on the Wizard's scroll, which are solved through kindness, creativity, and conversation rather than combat
- Arrange for your nosy neighbor to look after the farm, and say a proper goodbye to your beloved farm animal before you set out

Every game has new names, new quests, and new characters. A game is meant to be played in one sitting, and progress isn't saved between conversations. Going home is always an honorable ending.

## Install in Claude Code

Add this repository as a marketplace, then install the plugin:

```bash
claude plugin marketplace add srosebattles/fools-errand-game
claude plugin install fools-errand@fools-errand-game
```

Or do both from inside a Claude Code session:

```text
/plugin install fools-errand --marketplace srosebattles/fools-errand-game
```

## What's inside

This plugin contains a single skill, `fools-errand`, which is plain Markdown instructions for Claude. It has no scripts, hooks, MCP servers, or other executable code. It doesn't fetch anything, collect any data, or send anything anywhere. During play, the skill asks Claude not to use other tools, so the game stays in plain text.

```text
.claude-plugin/
  plugin.json        Plugin manifest
  marketplace.json   Lets Claude Code install the plugin from this repository
skills/
  fools-errand/
    SKILL.md         The game master instructions
LICENSE              CC BY 4.0
```

## License

A Fool's Errand by srosebattles is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0). The full text is in [LICENSE](LICENSE).

You're free to share and adapt it, including commercially, as long as you give credit and say if you made changes. If you publish a remix, please include a link back to [llmtextgames.xyz](https://llmtextgames.xyz) in your credit. For example:

> Based on *A Fool's Errand* by srosebattles ([llmtextgames.xyz](https://llmtextgames.xyz)), licensed under CC BY 4.0.
