# Bash
Bash, SH, Dash, Fish, Command Line, CMD

+ if dir not exist then make it.
  ```bash
  dir=pathToDir && [ ! -d $dir ] && [ ! -L $dir ] && mkdir $dir || echo " $dir > `readlink -f $dir` "
  ```

+ if file not exist then make it.
  ```bash
  file=file && [ ! -f $file ] && echo "$FILE does not exist." || echo "$FILE exist."
  ```
  
+ if package is not installed then install it.
  ```bash
  pkg=git && ! which $pkg > /dev/null && sudo apt install -y $pkg || echo "`which $pkg` is already installed."
  ```
