# nests
mappings for inner class attributes

## Nester mappings
In Minecraft versions 1.8.2-pre4 and below, any attributes that specified a relationship between inner classes and outer
classes were stripped by Mojang using ProGuard, adding an extra inconvenience to the process of parsing and mapping the
classes.
In an effort to remedy this, Matcher was [forked](https://github.com/OrnitheMC/matcher) and
[Nester](https://github.com/OrnitheMC/nester) was created in order to find and restore as many inner and outer class
attributes as reasonably possible.
In order to "re-nest" these classes in production, Nester mappings (with the `.nest` extension) have to be provided so Nester
can fix these classes automatically, of which can be found in the `nests` directory.
