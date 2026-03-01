# Neovim Cheatsheet                                                                                                                                                                         
                                                                                                                                                                                              
  > **Leader key:** `Space`                                                                                                                                                                   
                  
  ---                                                                                                                                                                                         
                  
  ## Basic Navigation

  ### Cursor Movement
  | Key | Action |
  |-----|--------|
  | `h` | Move left |
  | `j` | Move down |
  | `k` | Move up |
  | `l` | Move right |
  | `w` | Jump forward one word |
  | `b` | Jump backward one word |
  | `e` | Jump to end of word |
  | `0` | Jump to start of line |
  | `$` | Jump to end of line |
  | `gg` | Go to top of file |
  | `G` | Go to bottom of file |
  | `{` | Jump to previous empty line (paragraph up) |
  | `}` | Jump to next empty line (paragraph down) |
  | `Ctrl-d` | Scroll down half page |
  | `Ctrl-u` | Scroll up half page |
  | `zz` | Center current line on screen |

  ### Modes
  | Key | Action |
  |-----|--------|
  | `i` | Enter Insert mode (before cursor) |
  | `a` | Enter Insert mode (after cursor) |
  | `o` | Open new line below and enter Insert |
  | `O` | Open new line above and enter Insert |
  | `v` | Enter Visual mode |
  | `V` | Enter Visual Line mode |
  | `Ctrl-v` | Enter Visual Block mode |
  | `Esc` | Return to Normal mode |

  ### Editing
  | Key | Action |
  |-----|--------|
  | `dd` | Delete (cut) current line |
  | `yy` | Yank (copy) current line |
  | `p` | Paste after cursor |
  | `P` | Paste before cursor |
  | `u` | Undo |
  | `Ctrl-r` | Redo |
  | `x` | Delete character under cursor |
  | `r` | Replace character under cursor |
  | `ciw` | Change inner word |
  | `di"` | Delete inside quotes |
  | `.` | Repeat last action |

  ### Search
  | Key | Action |
  |-----|--------|
  | `/pattern` | Search forward |
  | `?pattern` | Search backward |
  | `n` | Next match |
  | `N` | Previous match |
  | `*` | Search word under cursor |
  | `:noh` | Clear search highlight |

  ---

  ## Window Management

  ### Split Navigation
  | Key | Action |
  |-----|--------|
  | `Ctrl-h` | Move to left window |
  | `Ctrl-j` | Move to bottom window |
  | `Ctrl-k` | Move to top window |
  | `Ctrl-l` | Move to right window |

  ### Split Resize
  | Key | Action |
  |-----|--------|
  | `F5` | Increase height |
  | `F6` | Decrease height |
  | `F7` | Increase width |
  | `F8` | Decrease width |

  ### Split Creation
  | Key | Action |
  |-----|--------|
  | `Space vs` | Vertical split + open next buffer |
  | `:sp` | Horizontal split |
  | `:vsp` | Vertical split |

  ---

  ## Buffer Management

  ### Navigation
  | Key | Action |
  |-----|--------|
  | `Shift-l` | Next buffer |
  | `Shift-h` | Previous buffer |
  | `Alt-1` … `Alt-9` | Go to buffer 1–9 |
  | `Alt-0` | Go to last buffer |

  ### Reordering
  | Key | Action |
  |-----|--------|
  | `Alt-Shift-h` | Move buffer left |
  | `Alt-Shift-l` | Move buffer right |
  | `Alt-p` | Pin/unpin current buffer |

  ### Closing
  | Key | Action |
  |-----|--------|
  | `Space q` | Close current buffer |
  | `Space Q` | Force close buffer |
  | `Space U` | Close all buffers |

  ---

  ## File & Search

  | Key | Action |
  |-----|--------|
  | `Space f` | Find files (current directory) |
  | `Space Fh` | Find files in home directory |
  | `Space Fc` | Find files in `~/.config` |
  | `Space Fl` | Find files in `~/.local/src` |
  | `Space Ff` | Find files above current directory |
  | `Space Fr` | Resume last search |
  | `Space g` | Grep current directory |
  | `Space G` | Grep word under cursor |

  ### Inside fzf-lua popup
  | Key | Action |
  |-----|--------|
  | `F1` | Toggle help |
  | `F2` | Toggle fullscreen |
  | `F4` | Toggle preview |
  | `Shift-Down` / `Shift-Up` | Scroll preview |
  | `Alt-a` | Toggle select all |
  | `Ctrl-z` | Abort |

  ---

  ## File Explorer (nvim-tree)

  | Key | Action |
  |-----|--------|
  | `Space t` | Toggle file explorer |
  | `g?` | Show all tree keybindings (inside tree) |

  ---

  ## File Operations

  | Key | Action |
  |-----|--------|
  | `Space w` | Save file |
  | `Space d` | Duplicate file (save with new name) |
  | `Space x` | Make file executable (`chmod +x`) |
  | `Space mv` | Move file to new directory |
  | `Space u` | Open URL under cursor in browser |

  ---

  ## Comments (Comment.nvim)

  | Key | Action |
  |-----|--------|
  | `gcc` | Toggle line comment |
  | `gb` | Toggle block comment |
  | `gcO` | Add comment on line above |
  | `gco` | Add comment on line below |
  | `gcA` | Add comment at end of line |
  | `gc{motion}` | Comment over motion (e.g. `gc3j`) |

  ---

  ## Terminal

  | Key | Action |
  |-----|--------|
  | `Space z` | Open floating terminal |
  | `Space H` | Open htop in floating terminal |
  | `Esc` | Close floating terminal (preserves session) |

  ---

  ## Git (Gitsigns)

  Signs appear automatically in the gutter for tracked files:
  - `┃` Added / Changed lines
  - `_` Deleted lines
  - `┆` Untracked

  | Command | Action |
  |---------|--------|
  | `:Gitsigns toggle_current_line_blame` | Toggle inline blame |
  | `:Gitsigns toggle_signs` | Toggle gutter signs |
  | `:Gitsigns toggle_word_diff` | Toggle word diff |

  ---

  ## Appearance & Editor

  | Key | Action |
  |-----|--------|
  | `Space p` | Cycle through themes (catppuccin → gruvbox → pywal16) |
  | `Space l` | Toggle Twilight (dim surrounding code) |
  | `Space nn` | Toggle relative / absolute line numbers |
  | `Space W` | Toggle line wrap |

  ---

  ## Config Management

  | Key | Action |
  |-----|--------|
  | `Space R` | Reload Neovim config |
  | `Space P` | Install plugins (`:PlugInstall`) |
  | `Space ma` | Run `make uninstall && make clean install` |

  ---

  ## CSV Files (decisive.nvim)

  | Key | Action |
  |-----|--------|
  | `Space csa` | Align CSV columns |
  | `Space csA` | Clear CSV alignment |
  | `[c` | Go to previous column |
  | `]c` | Go to next column |

  ---

  ## JS / TS / Bun

  ### Autocomplete (nvim-cmp)
  Suggestions appear automatically as you type from the language server, current file words, and file paths.

  | Key | Action |
  |-----|--------|
  | *(just type)* | Suggestions appear automatically |
  | `Tab` | Select next suggestion |
  | `Shift-Tab` | Select previous suggestion |
  | `Enter` | Confirm / accept suggestion |
  | `Ctrl-Space` | Force open suggestions |
  | `Ctrl-e` | Close the suggestion menu |

  ### LSP (typescript-language-server)
  Auto-activates for `.js`, `.jsx`, `.ts`, `.tsx` when a `tsconfig.json`, `jsconfig.json`, or `package.json` is found.

  | Key | Action |
  |-----|--------|
  | `gd` | Go to definition |
  | `gr` | Find references |
  | `K` | Hover documentation |
  | `[d` / `]d` | Previous / next diagnostic |
  | `:lua vim.lsp.buf.format()` | Format file |

  Linting via **eslint** runs automatically on save.

  > Install: `bun add -g typescript-language-server typescript`

  ### package-info.nvim (package.json helper)
  Open a `package.json` file, then:

  | Key | Action |
  |-----|--------|
  | `Space ns` | Show installed versions inline |
  | `Space np` | Hide versions |
  | `Space nu` | Update package under cursor |
  | `Space nd` | Delete package under cursor |
  | `Space ni` | Install a new package |
  | `Space nv` | Change version of package under cursor |

  Uses **bun** as the package manager.

  ---

  ## LSP (Go — gopls)

  Auto-activates for `.go` files. Also gets autocomplete via nvim-cmp.

  | Key | Action |
  |-----|--------|
  | `gd` | Go to definition |
  | `gr` | Find references |
  | `K` | Hover documentation |
  | `[d` / `]d` | Previous / next diagnostic |
  | `:lua vim.lsp.buf.format()` | Format file |

  Linting runs automatically on save for: Lua, Python, Shell, C, Rust, CSS, HTML, JS, TS.

  ---

  ## Go to Home Page (Alpha Dashboard)

  The Alpha dashboard appears automatically when:
  - Neovim launched with no file: `nvim`
  - All buffers are closed

  To manually return, close all buffers:
  ```
  :bd    ← delete current buffer (repeat until alpha appears)
  ```
  Or quit and reopen: `:qa` then `nvim`

  ### Alpha Dashboard Shortcuts
  | Key | Action |
  |-----|--------|
  | `e` | New empty file |
  | `f` | Find file (fzf-lua) |
  | `t` | Browse current directory (nvim-tree) |
  | `r` | Browse `~/.local/src` |
  | `s` | Browse `~/scripts` |
  | `c` | Open config directory |
  | `m` | Edit keybindings (`mappings.lua`) |
  | `p` | Install plugins |
  | `q` | Quit Neovim |

  ---

  ## Quick Reference Card

  ```
  MOVE       h j k l / w b e / gg G / { }
  MODES      i a o O / v V Ctrl-v / Esc
  EDIT       dd yy p u Ctrl-r / ciw .
  SEARCH     /pat n N * :noh
  COMPLETE   Tab/S-Tab navigate · Enter confirm · Ctrl-e close
  WINDOWS    Ctrl-h/j/k/l | F5-F8 resize
  BUFFERS    Shift-h/l | Alt-1..9 | Spc-q
  FILES      Spc-f/g/G | Spc-t (tree)
  SAVE       Spc-w | QUIT :q :qa :q!
  HOME       :bd until alpha appears · or :qa then nvim
  ```

