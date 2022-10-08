# Project Time In Time Out
## Master Media Design, HEAD – Genève
## [Alexia Mathieu](https://www.hesge.ch/head/annuaire/alexia-mathieu) & [Douglas Edric Stanley](http://abstractmachine.net)

### What Is This
This is our Twee (a.k.a. Twine) slideshow shown in the first day of class.

### How To Install
First download [Tweego](http://www.motoslave.net/tweego/) files somewhere onto your machine. Call this folder `SomeAwesomeName`.

Create a folder for your Twee project somewhere on your machine.

Copy from the Tweego folder, the `tweego` file and `storyformats` folder, into your `SomeAwesomeName` folder.

Open this folder in [VS Code](https://code.visualstudio.com). In VS Code install the [Twee 3 Language Tools](https://marketplace.visualstudio.com/items?itemName=cyrusfirheir.twee3-language-tools) extension (just click on that link, it will open VS Code).

Open a Terminal in VS Code: `Menu` > `Terminal` > `New Terminal`. Make the `tweego` file executable with this command in the Terminal: `chmod 755 tweego`.

### How To Use
Create a `story.twee` file in your folder.

Create inside that file a Starting block:

```
:: Start
This is my first Twine page
```

Convert your Twee file into a working webpage.

### How To Compile Multiple Files Into a Single Page
This project uses `story.twee` and a folder containing multiple `*.twee` files. Here is how to compile all those files into one single Twine project:

From the command line, type:

````
./tweego -o index.html story.twee passages
````