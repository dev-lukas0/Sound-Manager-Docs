## play

Plays a sound from the registry

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