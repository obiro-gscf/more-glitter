# IntelliJ Cheatsheet

## Importing a project from Github

File > New > Project from Version Control
URL - found on Github

> In some projects, the file paths might get too long for the operating system - if cloning your project fails, try changing the destination directory to a shorter path.

## Searching throughout the project

- *Find text* (search string) - Ctrl + Shift + F

> Pay attention to the search scope - in most cases, "In Project" is the one you need.

- *Search everywhere* - double Shift

> **When should you use *Find text* and when *Search everywhere*?**
> 
> In general: whichever is easier for you.
>
> *Find text* shows fragments of the code for each of the search result, which sometimes might help identifying whether the result is relevant or not.
>
> *Search everywhere* allows to also search for editor actions and IntelliJ-specific tools, not only contents of the files.

- *Find file* (by name) - Ctrl + Shift + N
- *Find class* (by name) - Ctrl + N

> You can use camel case to speed up your searching - IntelliJ will try to match each part of the case to a separate camel case part of the result.
>
>For example: when looking for `AbsolutelyComplicatedFileNameHere`, you can use following search terms:
>- `AbsolutelyComplicatedFileNameHere`
>- `AbsolutelyComplicated` (fully matched prefix)
>- `absolutelycomplicated` (works also lowercase)
>- `absCompFiNa` (each part of camel case is a prefix of the corresponding part in the result)
>- `ACFNH` (uppercase letter for each name part)

## Navigating code

- *Ctrl + click* -> depending on what object you click, it can navigate to
    - all the usages of a variable / method
    - the implementation of a method
    - the definition of a class
- *Go to implementation* - Ctrl + Alt + B
- *Go to usages* - Ctrl + B

> **When to use *Ctrl + click* and when *Go to implementation / usages*?**
> 
> *Ctrl + click* is the simplest to use and in most cases will lead you to the place you're looking for.
>
> However, in some cases (e.g. when code is using interfaces) *Ctrl + click* might lead to a dead-end - then the other shortcuts will give more options.

- *Go to the previously visited file* - Ctrl + Tab (if you hold the keys, you will see a list of previously visited files, you can navigate through them using Tab while holding Ctrl)
- *See recent files* - Ctrl + E
- *Go to previous place in code* - Ctrl + Alt + Left Arrow
- *Go to next place in code* - Ctrl + Alt + Right Arrow

> **What is the difference between the 4 options above?**
> 
> *See recent files* gives the most options, as it keeps the longest history of files viewed.
> 
> *Go to previously visited file* is fastest to switch in-between files.
> 
> *Go to previous / next place* allows to navigate within one file (especially useful for long files!)

Of course, the standard shortcuts for copy / paste are also working in IntelliJ.

> [!tip] IntelliJ keeps a history of pasted text - you can use Ctrl + Shift + V to view it (and choose which contents will be pasted)!

## Git operations

- `git pull` -> Update Project
- `git commit` -> Commit... / Ctrl + K
- `git push` -> Push... / Ctrl + Shift + K
- `git checkout` -> Pick a branch from a dropdown, right click, select Checkout
- `git rebase` -> available from Git toolbar in the bottom
- `git blame` -> In editor window, right click next to the line number and select *Annotate with Git Blame*
- stashing -> useful during interruptions, to quickly "clean up" the local code state without losing changes - In Commit toolbar, select all the relevant changes, right click and select *Shelve changes...* - after the operations, all your progress will appear in "Shelf" tab in the sam toolbar

## Additional resources

Help > Keyboard Shortcuts PDF

IntelliJ documentation [website](https://www.jetbrains.com/help/idea/getting-started.html)

IntelliJ offers also an in-editor training course for learning the essential features, details can be found [here](https://www.jetbrains.com/help/idea/feature-trainer.html)