# Bash
Bash, SH, Dash, Fish, Command Line, CMD

+ if dir not exist then make it.
  ```bash
  dir=path/to/dir && [ ! -d $dir ] && [ ! -L $dir ] && mkdir $dir || echo " $dir > `readlink -f $dir` "
  ```
