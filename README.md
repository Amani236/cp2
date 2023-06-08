# cp2
dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again
$ git init
Initialized empty Git repository in C:/Users/dell/Desktop/learn_git_again/.git/

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git add .

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git commit -m 'adding third.txt'
[master (root-commit) 5ab587d] adding third.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 third.txt

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git log
commit 5ab587de1854715a084f9711bfef27bfe21b11db (HEAD -> master)
Author: Amani236 <belloumiamani70@gmail.com>
Date:   Thu Jun 8 11:09:42 2023 +0100

    adding third.txt

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git add fourth.txt

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git commit -m 'adding fourth.txt'
[master e26aa97] adding fourth.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 fourth.txt

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git rm --cached third.txt
rm 'third.txt'

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git add .

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git commit -m 'removing third.txt'
On branch master
nothing to commit, working tree clean

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git add .

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git commit -m ''
On branch master
nothing to commit, working tree clean

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git add .

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git commit -m ''
On branch master
nothing to commit, working tree clean

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git add .

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git commit -m ''
Aborting commit due to empty commit message.

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git commit -m 'thirdp'
[master 80df8d8] thirdp
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename third.txt => third'.txt (100%)

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git add .

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git commit -m 'third -'
[master d29a7b8] third -
 1 file changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 third'.txt

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git log
commit d29a7b893138efeb04bf96fe82b5424b3e651029 (HEAD -> master)
Author: Amani236 <belloumiamani70@gmail.com>
Date:   Thu Jun 8 11:26:12 2023 +0100

    third -

commit 80df8d87e0872c2af01a241eb9df4029dec588e7
Author: Amani236 <belloumiamani70@gmail.com>
Date:   Thu Jun 8 11:25:08 2023 +0100

    thirdp

commit e26aa9712aa015e4ec7f6d37910adbbed8190799
Author: Amani236 <belloumiamani70@gmail.com>
Date:   Thu Jun 8 11:10:54 2023 +0100

    adding fourth.txt

commit 5ab587de1854715a084f9711bfef27bfe21b11db
Author: Amani236 <belloumiamani70@gmail.com>
Date:   Thu Jun 8 11:09:42 2023 +0100

    adding third.txt

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git log oneline
fatal: ambiguous argument 'oneline': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git log --oneline
d29a7b8 (HEAD -> master) third -
80df8d8 thirdp
e26aa97 adding fourth.txt
5ab587d adding third.txt

dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$ git config --global
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    --worktree            use per-worktree config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-pattern]
    --get-all             get all values: key [value-pattern]
    --get-regexp          get values for regexp: name-regex [value-pattern]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value-pattern]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-pattern]
    --unset-all           remove all matches: name [value-pattern]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    --fixed-value         use string equality when comparing values to 'value-pattern'
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    -t, --type <type>     value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --bool-or-str         value is --bool or string
    --path                value is a path (file or directory name)
    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)
    --show-scope          show scope of config (worktree, local, global, system, command)
    --default <value>     with --get, use default value when missing entry


dell@DESKTOP-OBBQDOU MINGW64 ~/Desktop/learn_git_again (master)
$
