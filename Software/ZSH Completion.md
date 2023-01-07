#zsh #linux #software 

[zsh-completions/zsh-completions-howto.org at master · zsh-users/zsh-completions](https://github.com/zsh-users/zsh-completions/blob/master/zsh-completions-howto.org#intro)

## My first custom completion

```bash
_arguments '-e[edit existing script]:filename:->files' '-d[delete existing script]:filename:->files' 

case "$state" in
  files)
    local -a scripts
    scripts=( $(find ~/.local/bin/ -type f -maxdepth 1 -exec basename {} \;) )
    _values 'scripts' $(find ~/.local/bin/ -type f -maxdepth 1 -exec basename {} \;)
  ;;
esac
```