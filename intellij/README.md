# ReSharper/VisualStudio/OSX Keymap for Intellij IDEA

Default Intellij keymap is based on Borland. That's way too old. ReSharper has the best keymap I've yet to bump into on an IDE, and Visual Studio makes some sense as well.

I've combined the two and made it work for OSX.

### Contributing

You'll need to Export Settings, and unpack the `setting.jar` it spits out (it's a regular zip). Within it, find your XML keymap file under the `keymaps` folder, and overwrite the one in this repository.

Next, make a commit and submit a pull request which I will gladly accept.

Thanks! :)

### Building

To get an up-to-date jar, just run ./build.sh. Then you can import it to Intellij.
