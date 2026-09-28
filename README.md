# maven

A static Maven repository, served by GitHub Pages at <https://msameer.github.io/maven/>, for
`dev.msameer.vaw:vaw-api`: the API that extensions of the
[Villagers at Work](https://www.curseforge.com/minecraft/mc-mods/villagers-at-work) mod build against.
Villagers at Work's CI publishes to it; nothing here is edited by hand.

```kotlin
repositories {
    maven("https://msameer.github.io/maven/")
}

dependencies {
    compileOnly("dev.msameer.vaw:vaw-api:0.10.4+26.2")
}
```

Versions are `<api version>+<Minecraft release>`; `-SNAPSHOT` builds come from the mod's main branch.

## Licence

The api is MIT. See [LICENSE](LICENSE).
