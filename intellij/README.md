# ReSharper/VisualStudio/OSX Keymap for Intellij IDEA

Default Intellij keymap is based on Borland. That's way too old. ReSharper has the best keymap I've yet to bump into on an IDE, and Visual Studio makes some sense as well.

I've combined the two and made it work for OSX.

## Notable Keymaps

* `cmd + M` - expanding selection (word/line/paragraph)
* `cmd + Space` - Smart Completion by default
* `cmd + R` - Refactor. Like ReSharper (`cmd + R,V` / `cmd + R,R`)
* `cmd + E` - Extract. Like ReSharper (`cmd + E,U` etc)

_Navigation_


* `Shift + Return` - Move to next line without breaking
* `cmd + T` / `cmd + P` - navigate to anything (intellij's 'to type')
*  `cmd + shift + I` - Go to start of line, like vim's `shift + I`
*  `cmd + shift + A` - Go to end of line, like vim's `shift + A`
* `cmd + shift + {h,j,k,l}` - navigate left,down,up,right from home row (like vim's visual mode navigation)
* `cmd + shift + {b,w}` - previous word, next word (like vim's visual mode b,w for previous and next word)

## Why not just use Intellij-Vim?

I wish. Because it's buggy and messy when you want to include ReSharper multi-step
shortcuts in addition to existing editor shortcuts; belive me, I've tried :(

If you still think otherwise - please create an issue - I'd like to hear
about it.

### Contributing

You'll need to Export Settings, and unpack the `setting.jar` it spits out (it's a regular zip). Within it, find your XML keymap file under the `keymaps` folder, and overwrite the one in this repository.

Next, make a commit and submit a pull request which I will gladly accept.

Thanks! :)

### Building

To get an up-to-date jar, just run ./build.sh. Then you can import it to Intellij.
