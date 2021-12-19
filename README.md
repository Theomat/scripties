# scripties

A compilation of useful scripts that I use.

If the license is unspecified or if no credit is given in the script, then the code is mine and under public domain.
Otherwise, please check out the given link or the information given in the file to see which license applies to the specified program.

<!--toc-->
- [Bash scripts](#bash-scripts)
  - [Autolink](#autolink)
  - [Ex](#ex)
  - [Spawn](#spawn)
- [Python scripts](#python-scripts)
  - [Pydeps](#pydeps)
- [Ruby scripts](#ruby-scripts)
- [Easy Install](#easy-install)

<!--end toc-->

---

## Bash scripts

### Autolink

Location: ```bash/autolink```

Usage: ```autolink <folder_src> <folder_dst>```

Description: Find all executables files in a recursive manner from `folder_src` and for each create a symbolic link in `folder_dst` with the file's name. Note that it automatically ignores git files.

### Ex

Location: ```bash/ex```

Usage: ```ex <file>```

Description: Extract the files from the specified archive based on its extension, it is already present in some distributions' default ```.bashrc```.

### Spawn

Location: ```bash/spawn```

Usage: ```spawn cmd```

Description: Spawn the specified ```cmd``` as a detached process of the current terminal using ```nohup``` (GNU).

---

## Python scripts

### Pydeps

Location: ```python/pydeps```

Usage: ```pydeps -h```

Description: Automatically find and list python dependencies in a requirements.txt fashion.

---

## Ruby scripts

Location: ```ruby/colt```

Usage: ```colt -h```

Description: Translates the given colors from one color space to another.

Supports: rgb, bgr, hsv, bw, grayscale

---

## Easy Install

If you have a folder `DST` that's in your `PATH`, what you can do once you have cloned this repository is run:

```bash
./scripties/bash/autolink ./scripties DST
```

This will create symlinks from all of the scripts in the scripties into your `DST` folder enabling you to run them directly from the command line.
