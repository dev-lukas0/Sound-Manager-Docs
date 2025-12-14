## stop

Stops a sound that is currently playing

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
task.wait(1);
Sounds.stop("SCP096");
```

## stopAll

Stops all currently playing sounds
Usage:
```ts
Sounds.stopAll();
```