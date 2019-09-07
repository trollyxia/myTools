# myTools



## Git config:

[.gitconfig](.gitconfig)



## Diff tool:

An improved colored diff: [icdiff](https://github.com/jeffkaufman/icdiff)

#### Installation: 

- Download the [latest](https://github.com/jeffkaufman/icdiff/releases) `icdiff` binary and put it on your PATH.

- Alternatively, install with pip:

  ```shell
  pip install git+https://github.com/jeffkaufman/icdiff.git
  ```

#### Usage:

````shell
icdiff [options] left_file right_file
git icdiff [options] left_file right_file
````

Show differences between files in a two column view.