## mach boom study
* download deps
```zsh
mach dep pull .
```
## Set project.src path in mach.toml
```toml
[project]
src = "src" # or "src-cn"
```
## Use Makefile
```zsh
# set makefile SRC_ROOT = src # or src-cn
# set makefile ARGS = libs/path
make
# or
make file_name

# run
make run file_name
# or
make run file_name ARGS="-L libs/path" 
```
## Use Mach
```zsh
# build
mach build . -a file_name
# or
mach build . -L libs/path -a file_name

# run
mach run . -a file_name
```
