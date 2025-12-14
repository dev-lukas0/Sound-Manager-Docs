## fadeIn

Fades in a sound over a specified duration

function:
```ts
function fadeIn(soundName: SoundName, duration: number, volume: number)
```

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
Sounds.fadeIn("SCP096", 2, 1);
```

## fadeOut

Fades out a sound over a specified duration
function:
```ts
function fadeOut(soundName: SoundName, duration: number, targetVolume?: number)
```

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
Sounds.fadeOut("SCP096", 2);
```

:::info targetVolume
The `targetVolume` parameter is optional. If not provided, it defaults to 0. Normally used when you want to fade out to a specific volume instead of completely silencing the sound.
:::