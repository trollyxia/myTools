# myTools



## Git config:

- My git config: [.gitconfig](.gitconfig)

- To show git branch name in linux directory, add the following code in `~/.bashrc`:

  ```shell
  function git_branch {
          branch="`git branch 2>/dev/null | grep "^\*" | sed -e "s/^\*\ //"`"
          if [ "${branch}" != "" ];then
                  if [ "${branch}" = "(no branch)" ];then
                          branch="(`git rev-parse --short HEAD`...)"
                  fi
                  echo " ($branch)"
          fi
  }
  
  export PS1='\u@\h \[\033[01;36m\]\w\[\033[01;32m\]$(git_branch)\[\033[00m\] \$ '
  ```



## Markdown tool:

A markdown editor: [Typora](https://www.typora.io/)



## Snipaste:

A screenshot tool and pin the screenshot to the desk: [Snipaste](https://zh.snipaste.com/)

#### Usage:

- `F1` to take a screenshot, `F3` to pin the screenshot to the desk.

- `shift` + `double click` to minimize the picture.



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