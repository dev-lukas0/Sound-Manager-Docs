## onEnd

Registers a callback function to be called when a sound ends playing

function:
```ts
function onEnd(soundName: SoundName, callback: () => void)
```

Usage:
```ts
Sounds.onEnd("SCP096", () => {
    print("Hello world!");
})
```

:::danger
The onEnd function is still in development and not usable yet.
:::