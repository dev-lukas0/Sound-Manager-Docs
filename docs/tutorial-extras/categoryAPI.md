# Sound-Category API

## loadCategory
Ensures all sounds in a specified Sound-Category are loaded into `ReplicatedStorage`.

Function:
```ts
function loadCategory<C extends SoundCategory>(category: C): void;
```

Usage:
```ts
SoundCategories.loadCategory("Menu");
```

## playCategory
Plays all sounds within a specified Sound-Category.

Function:
```ts
function playCategory<C extends SoundCategory>(category: C): void;
```
Usage:
```ts
SoundCategories.playCategory("Menu");
```
## stopCategory
Stops all sounds within a specified Sound-Category.

Function:

```ts
function stopCategory<C extends SoundCategory>(category: C): void;
```
Usage:
```ts
SoundCategories.stopCategory("Menu");
```

## stopAllCategories
Stops all sounds within all Sound-Categories.

Function:
```ts
function stopAllCategories(): void;
```
Usage:
```ts
SoundCategories.stopAllCategories();
```

## setCategoryVolume
Sets the volume for all sounds within a specified Sound-Category.

Function:
```ts
function setCategoryVolume<C extends SoundCategory>(category: C, volume: number): void;
```
Usage:
```ts
SoundCategories.setCategoryVolume("Menu", 0.5);
```

## setGlobalCategoryVolume
Sets the global volume for all categories.

Function:
```ts
function setGlobalCategoryVolume(volume: number): void;
```
Usage:
```ts
SoundCategories.setGlobalCategoryVolume(0.8);
```

## isCategoryPlaying
Checks if all sounds in a category are currently playing.

Function:
```ts
function isCategoryPlaying<C extends SoundCategory>(category: C): boolean;
```
Usage:
```ts
const playing = SoundCategories.isCategoryPlaying("Menu");
```

## playSoundFromCategory
Plays a specific sound from a category. Autocompletion ensures only valid sound names can be used.

Function:
```ts
function playSoundFromCategory<C extends SoundCategory, S extends keyof T[C]["sounds"]>(category: C, sound: S): void;
```
Usage:
```ts
SoundCategories.playSoundFromCategory("Menu", "Click");
```

## resetCategory
Resets all sounds in a category to their starting position.

Function:
```ts
function resetCategory<C extends SoundCategory>(category: C): void;
```

Usage:
```ts
SoundCategories.resetCategory("Menu");
```

## resetAllCategories
Resets all sounds in all categories to their starting position.

Function:
```ts
function resetAllCategories(): void;
```

Usage:
```ts
SoundCategories.resetAllCategories();
```
## preloadCategory
Preloads all sounds in a category.

Function:
```ts
function preloadCategory<C extends SoundCategory>(category: C): void;
```
Usage:
```ts
SoundCategories.preloadCategory("Menu");
```

## preloadAllCategories
Preloads all sounds in all categories.

Function:
```ts
function preloadAllCategories(): void;
```
Usage:
```ts
SoundCategories.preloadAllCategories();
```

## fadeInCategory
Gradually increases the volume of all sounds in a category over a duration.

Function:
```ts
function fadeInCategory<C extends SoundCategory>(category: C, duration: number, volume: number): void;
```
Usage:
```ts
SoundCategories.fadeInCategory("Menu", 2, 1);
```

## fadeOutCategory
Gradually decreases the volume of all sounds in a category over a duration, optionally stopping them at zero.

Function:
```ts
function fadeOutCategory<C extends SoundCategory>(category: C, duration: number, targetVolume?: number): void;
```
Usage:
```ts
SoundCategories.fadeOutCategory("Menu", 2);
```

## onCategoryEnd
Registers a callback to be executed when all sounds in a category finish playing.

Function:
```ts
function onCategoryEnd<C extends SoundCategory>(category: C, callback: () => void): void;
```
Usage:
```ts
SoundCategories.onCategoryEnd("Menu", () => {
    print("All Menu sounds finished!");
});
```