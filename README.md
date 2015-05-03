zsh-vi-done-right
=================

Complete vi mode for zsh.

![zsh-vi-done-right](https://github.com/oselivanov/zsh-vi-done-right/raw/master/demo.gif)

Features:
 - Really cool 2-line colored prompt with current mode (command/insert) showing.
   Having 2 lines is very useful because position of the command is consistent.
 - Prompt with main color changing (blue to red) when using .zsh_vi over the ssh
   (through zsh_vi_i_am_home setting).
 - Better rensponsivity and removing zsh stuck when you accidentaly hit Esc in
   command mode.
 - Fixed zsh issue when you cannot delete text using backspace in cmd mode.
 - Word walking.
 - Better incremental search with / in command mode
   (^n and ^p used to go to next and previous match).
 - Use ^h to go one level up.
 - Disabled moving one char back after switching to insert mode.
 - Use e in command mode to edit current command line with vim.
 - Lighting fast git branch and current python virtualenv showing in prompt.
 - Clear screen with ^L without losing previous lines.
 - Showing finishing notification for long-running commands in Mac OS.

Installation:
1)

  mkdir -p ~/.zsh
  cd ~/.zsh
  git clone https://github.com/oselivanov/zsh-vi-done-right.git

2) Add

  # zsh_vi_word_walking=1  # Optional.
  if [ -f ~/.zsh/zsh_vi_mode ]; then
    . ~/.zsh/zsh_vi_mode
  fi

to your .zshrc
