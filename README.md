**Grakkit** - It's the fusion of GraalVM, JavaScript, and Minecraft.

![Code Demo](./demo.gif)

If you want to get in touch with the community, join our [discord server](https://discord.gg/e682hwR) and we can assist you with whatever problem you may have.

# Getting Started

## IMPORTANT
Grakkit was designed to run on standard JDK, which means it comes pre-packaged with the GraalJS engine! This pre-packaged engine WILL conflict with the GraalVM JVM, so please use standard JDK to run servers running Grakkit!

## Installation
Head on over to the [releases](https://github.com/grakkit/grakkit/releases) page and grab the latest version for your platform. After that, just drop the JAR in whatever **plugins**, **mods**, or **extensions** folder you would install any other plugin, mod, or extension.

## Your First Project (Bukkit/Spigot/Paper)
Upon starting or reloading the server with the plugin installed, the `plugins/grakkit` folder will be created on your server. This is where most if not all development will take place, and serves as your home when working within the scope of grakkit.

Now, unless you know EXACTLY what you're doing (mad respect if you do) you should install the `@grakkit/stdlib-paper` package, a standard library for JavaScript development. Make sure you have NodeJS installed on your system, then navigate to `plugins/grakkit` in a terminal or command prompt and use `npm install @grakkit/stdlib-paper` to install it.

For those working on a remote server, you can simply install the `@grakkit/stdlib-paper` package to a local directory, then copy that directory's contents to the remote server's `plugins/grakkit` folder. This works because grakkit itself doesn't need NodeJS installed, it's merely the system we use for package management.

Once that's done, you can import it from within your main file (default `index.js`) as shown below...
```js
const stdlib = require('@grakkit/stdlib-paper');
```

...and upon the next server reload, the above code will be executed. This package also adds the in-game `/js` command, which can be used to test and execute code from within the game -- for example, `/js self` represents the player or console sending the command, and you can use `/js core.reload()` to reload the JS environment without having to reload the entire server.k

## Your First Project (Minestom)
Grakkit for [Minestom](https://github.com/Minestom/Minestom) is available as a standalone "extension." Download it from our [latest release]() page. Make sure to download the correct platform, labeled `grakkit-x.y.z.minestom.jar`.
The installation process and usage is very similar to that of bukkit/spigot/paper's, however the two key differences are **a).** it's an _extension_ and should be placed in the extensions directory rather than plugins, and **b).** it uses different modules to complete the Environment???, notably-being `@grakkit/stdlib-minestom`.

Grakkit for Minestom is still in its early days, however it's the best we've got as far as scripting in a performant environment like Minestom.

## Other Platforms
Grakkit is currently only available for servers implementing the Bukkit or Minestom's API. Check out [Other Implementations](https://github.com/grakkit/grakkit/wiki/Other-Implementations) to find alternatives for your platform!

## Further Reading
For more info about Grakkit, modules, the JS command, and more, head on over to the [wiki](https://github.com/grakkit/grakkit/wiki) and read up. ***Attention:** This wiki is slightly outdated and only applies to servers. Many of the code samples in here may still work, but some may not. Use at your own risk!*

For another useful guide to getting started, check out [Start Your Environment](https://github.com/grakkit/grakkit/wiki/HowTo-Start-Environment).
---

*Owned and maintained by [RepComm](https://github.com/RepComm) and [hb432](https://github.com/hb432). Special thanks to [brayjamin](https://github.com/brayjamin), [TonyGravagno](https://github.com/TonyGravagno), [dustinlacewell](https://github.com/dustinlacewell), [wagyourtail](https://github.com/wagyourtail), and [waterquarks](https://github.com/waterquarks) for their contributions to the project.*
 
