# Sound-Category

A Sound-Category is a group of sounds that can be managed together. This allows you to control the volume, looping, and other properties of a group of sounds at once.

## Creating a Sound-Category
To create a Sound-Category, you can use the `createSoundCategoryRegistry` function from the Sound-Manager library.

```ts
import { createSoundCategoryRegistry } from "@rbxts/sound-manager";

const SoundCategories = createSoundCategoryRegistry({
    Menu: {
        category: "Menu",
        sounds: {
            Click: {
                id: "rbxassetid://1234567890",
                volume: 0.5,
                loop: false,
            },

            Hover: {
                id: "rbxassetid://0987654321",
                volume: 0.5,
                loop: false,
            }
        }
    }
})
```


:::danger Note
The Sound-Category feautre is still in development
:::