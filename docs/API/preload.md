## preload
Preloads a specific sound in the registry

Usage:
```ts
Sounds.preload("SCP096");
```

## preloadAll
Preloads all sounds in the registry

Usage:
```ts
import { createSoundRegistry } from "@rbxts/sound-manager";

const Sounds = createSoundRegistry({
    SCP096: {
        id: "rbxassetid://4714389545",
        volume: 1,
        loop: false,
    } 
});

Sounds.preloadAll();

Sounds.play("SCP096");
```