git-cola v2.1.2 (unreleased)
============================

Usability, bells and whistles
-----------------------------
* Updated zh_TW translations.

* `git cola rebase` now defaults to `@{upstream}`, and generally uses the same
  CLI syntax as `git rebase`.

* The commit message editor now allows you to bypass commit hooks by selecting
  the "Bypass Commit Hooks" option.  This is equivalent to passing the
  `--no-verify` option to `git commit`.

  https://github.com/git-cola/git-cola/issues/357

* We now prevent the "Delete Files" action from creating a dialog that does
  not fit on screen.

  https://github.com/git-cola/git-cola/issues/378

* `git xbase` learned to edit rebase instruction sheets that contain
  `exec` commands.

* The diff colors are now configurable.  `cola.color.{text,add,remove,header}`
  can now be set with 6-digit hexadecimal colors.
  See the `git cola manual <https://git-cola.readthedocs.org/en/latest/git-cola.html#configuration-variables>_`
  for more details.

Fixes
-----
* `git cola` will now allow starting an interactive rebase with a dirty
  worktree when `rebase.autostash` is set.

  https://github.com/git-cola/git-cola/issues/360
