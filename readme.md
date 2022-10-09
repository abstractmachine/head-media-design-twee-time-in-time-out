# Project Time In Time Out
## Master Media Design, HEAD – Genève
## [Alexia Mathieu](https://www.hesge.ch/head/annuaire/alexia-mathieu) & [Douglas Edric Stanley](http://abstractmachine.net)

### What Is This?
This is our Twee (a.k.a. Twine) presentation shown in the first day of class.

---

### Play This Presentation
If you just want to play this presentation without changing anything, you can download the [latest release](https://github.com/abstractmachine/head-media-design-twee-time-in-time-out/releases/latest/) and open the `index.html` file (`Menu` > `File` > `Open File`) in your local browser.

### Local server
If your browser doesn't want to play nicely with this presentation, open this project folder in VS Code and run the [Live Server Extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)'s `Go Live` command (cf. bottom left of your code window).

---

### Watch Mode
We can let `Tweego` run in the background and build our project for us automatically whenever we make a change. I.e. `Tweego` will constantly watch the folder for changes, and automatically rebuild your project for you. If you are running `LiveServer` via the `Go Live` command, your project will immediately be updated in your browser on any save of any file in the project. To run this constant "Watch Mode", run the following command in your Terminal:

````
./tweego -w -o index.html story.twee passages css
````

To stop this "watch mode", do as it says in the console: type the `CTRL` + `C` keys.

---

### How To Create A Twee Project From Scratch
This project has already configured everything for you. If you want, you can also create a project from scratch. 

First download the [Tweego](http://www.motoslave.net/tweego/) files somewhere onto your machine.

Create a folder for your Twee project somewhere on your machine. Let's call this folder `SomeAwesomeName`.

From the Tweego folder you downloaded, copy both the `tweego` file and the `storyformats` folder (along with its contents) into this new `SomeAwesomeName` folder.

Open the folder `SomeAwesomeName` in [VS Code](https://code.visualstudio.com) : `Menu` > `File` > `Open Folder`.

Inside of VS Code, install the [Twee 3 Language Tools](https://marketplace.visualstudio.com/items?itemName=cyrusfirheir.twee3-language-tools) extension (just click on the link, it will open VS Code).

Also inside of VS Code, install the [Live Server Extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer). This will allow you to easily test your Twine stories directly in the browser of your choice. It will also reload the test page each time you save a change to any file in your project folder.

### Transform tweego into an executable command
`Tweego` takes our Twine code and turns it into a functioning webpage. To do this, we need to made `Tweego` an executable script from the command line. Open a Terminal in VS Code: `Menu` > `Terminal` > `New Terminal`. Make the `tweego` file executable with this command in the Terminal: `chmod 755 tweego`.

### How To Make a Tweego Project (easy version)
Create a `story.twee` file in your `SomeAwesomeName` folder.

Inside that text file, create a `Start` block:

````
:: Start
This is my first Twine page
````

Convert this Twee file into a working webpage:

````
./tweego -o index.html story.twee
````

### How To Compile Multiple Files Into a Single Project (fancy version)
This project uses:

- a main `story.twee` file
- several styles files in the `styles`folder
- a folder named `passages` containing multiple `*.twee` files

Here is how to compile all those files into one single Twine project. Open the Terminal: `Menu` > `Terminal` > `New Terminal`. From this Terminal, type:

````
./tweego -o index.html story.twee passages css
````

---

### To Do
- Add video controls
- Improve video layout