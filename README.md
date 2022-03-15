# Bash
Bash, SH, Dash, Fish, Command Line, CMD

+ if dir not exist then make it.
  ```bash
  dir=path/to/dir && [ ! -d $dir ] && [ ! -L $dir ] && mkdir $dir || echo " $dir > `readlink -f $dir` "
  ```
+ if package is not installed then install it.
  ```bash
  pkg=git && ! which  > /dev/null && sudo apt install $pkg || echo "$pkg already installed."
  ```
