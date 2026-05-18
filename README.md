# amlmarketplaces/elevenlabs

Claude Code marketplace federating all `@amlplugins/elevenlabs-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-elevenlabs": {
      "source": { "source": "github", "repo": "amlmarketplaces/elevenlabs" }
    }
  },
  "enabledPlugins": {
      "elevenlabs-audio-isolation@aml-elevenlabs": true,
      "elevenlabs-conversational-ai@aml-elevenlabs": true,
      "elevenlabs-dubbing@aml-elevenlabs": true,
      "elevenlabs-music@aml-elevenlabs": true,
      "elevenlabs-sound-effects@aml-elevenlabs": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/elevenlabs`, cached under `~/.claude/plugins/cache/aml-elevenlabs/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (10 total)

- `elevenlabs-audio-isolation` — [@amlplugins/elevenlabs-audio-isolation](https://github.com/amlplugins/elevenlabs-audio-isolation)
- `elevenlabs-conversational-ai` — [@amlplugins/elevenlabs-conversational-ai](https://github.com/amlplugins/elevenlabs-conversational-ai)
- `elevenlabs-dubbing` — [@amlplugins/elevenlabs-dubbing](https://github.com/amlplugins/elevenlabs-dubbing)
- `elevenlabs-music` — [@amlplugins/elevenlabs-music](https://github.com/amlplugins/elevenlabs-music)
- `elevenlabs-sound-effects` — [@amlplugins/elevenlabs-sound-effects](https://github.com/amlplugins/elevenlabs-sound-effects)
- `elevenlabs-stt` — [@amlplugins/elevenlabs-stt](https://github.com/amlplugins/elevenlabs-stt)
- `elevenlabs-tts` — [@amlplugins/elevenlabs-tts](https://github.com/amlplugins/elevenlabs-tts)
- `elevenlabs-voice-conversion` — [@amlplugins/elevenlabs-voice-conversion](https://github.com/amlplugins/elevenlabs-voice-conversion)
- `elevenlabs-voice-design` — [@amlplugins/elevenlabs-voice-design](https://github.com/amlplugins/elevenlabs-voice-design)
- `elevenlabs-voices` — [@amlplugins/elevenlabs-voices](https://github.com/amlplugins/elevenlabs-voices)

## Related

- npm packages: `@amlplugins/elevenlabs-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
