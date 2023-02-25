# Cat Commands

In this project I implemented three cat commands in window using nodejs.
We retrieve commands from CLI using `process` array.


- cat f1.txt => show the output of the file f1.txt
- cat f1.txt f2.txt => show the contents of file f1.txt and f2.txt together


## Flags 🏁

Example file <kbd>text.txt</kbd> :   
    
```
Hey i am f1
        


Bye i am f1
```

- -s flag : This flag is used to remove extra spaces from the output
    > Output when we apply s flag on f1.txt ⇒
    ```
    Hey i am f1

    Bye i am f1
    ```
    
- -b : This flag is used to add a line number on non empty lines
    > Output when we apply b flag on f1.txt ⇒
    ```
    1.Hey i am f1
            


    2.Bye i am f1
    ```

- -n : This flag is used to add a line number on all the lines including empty lines
    > Output when we apply n flag on f1.txt ⇒
    ```
    1.Hey i am f1
    2.
    3.
    4.
    5.Bye i am f1
    ```

- -b and -n flag are exclusive so the flag which has a lower index will be considered !

## Tech Stack ⚒

**Javascript, Node.js & FS Module**