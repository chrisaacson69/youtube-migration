# YouTube Migration
> Turning vault research into YouTube scripts — putting ideas into the ether and letting them fall where they do.

**Vault:** [Vault project page](https://github.com/chrisaacson69/Vault/blob/master/projects/youtube-migration/README.md)
**Tools:** [animation-studio](https://github.com/chrisaacson69/animation-studio)
**Infrastructure:** [animation-studio-pod](https://github.com/chrisaacson69/animation-studio-pod)

## Structure

```
series/                    # Episodes organized by series/playlist
├── philosophy/            # Logic, morality, epistemology
│   ├── ep01-.../
│   │   ├── script.md      # Episode script
│   │   └── scenes/        # Manim scene files
│   ├── ep02-.../
│   └── ...
├── math/                  # Numbers, infinity, measurement
└── economics/             # Markets, value, calculation

assets/                    # Shared across episodes
├── characters/            # Base PNGs + mouth variants
├── backgrounds/           # Scene backgrounds
└── music/                 # Background music

cloud-studio-spec.md       # RunPod production environment spec
```

## Episodes

| # | Series | Title | Status |
|---|--------|-------|--------|
| 1 | Philosophy | You Don't Know What Logic Is | In production — cold open rendered |

## Production Pipeline

1. **Script** (from Vault research) → defines content
2. **Voiceover** (TTS placeholder or recorded) → defines timing
3. **Manim scenes** (timed to voiceover) → animated content
4. **Character art** (ComfyUI + mouth overlays) → lip-synced characters
5. **Composite** (ffmpeg/moviepy) → final video
6. **Publish** → YouTube
