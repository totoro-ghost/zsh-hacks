# zsh-hacks ✨

## Resources

- [Official `zsh` website](https://zsh.sourceforge.io/)
- [`zsh` guide](https://zsh.sourceforge.io/Guide/)
- [`zsh` refcard](https://zsh.sourceforge.io/Refcard/)


## Some tips 🚀

- Don't use `oh-my-zsh`, why?
  - it add too many alias
  - it makes some things hard to modify
  - you have to learn how to change the prompt
  - if you don't know how it works, it's hard to make changes
  - you can do everything it does easily
- use a bare `.zshrc` - here is what i use - [`.zshrc`](./.zshrc)
- get list of all alias -> `print -rl -- ${(k)aliases}`
- get list of all functions you use -> `print -rl -- ${(k)functions}`
- run the original command instead of the alias -> type it inside single quotes, e.g. - `'ls'`
- is `zsh` starting slow?? - find out using `/usr/bin/time zsh -i -c exit`
- profiling `zsh` add `zmodload zsh/zprof` to top of `.zshrc` and `zprof` to bottom **OR**
  - use `zsh -xv` and see which part is taking more time while loading.
- here are some `zsh` plugins you should use
  - `zsh-syntax-highlighting`
  - `zsh-autosuggestions.zsh`
  - `zsh_command_not_found`