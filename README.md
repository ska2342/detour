# Detour for Emacs

An Emacs package to take a quick detour and come back.

# Use-Case

This Emacs package allows you to remember your current cursor
position, go somewhere else and then jump between those two
positions. It is meant for quick detours and then continuing your work
where you left off.

Suggested keybindings:

    (global-set-key [(control \.)] 'detour-mark)
    (global-set-key [(control \,)] 'detour-back)

Or via use-package:

    (use-package detour
      :bind
      ([(control \.)] . detour-mark)
      ([(control \,)] . detour-back))

Internally, a register is used to store the position. If you
manually set this register, these functions will not work.

# License

This is Free Software published under the GNU General Public License
version 2 or later (at your option).
