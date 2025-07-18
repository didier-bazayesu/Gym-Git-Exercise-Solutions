# Bundle 1 - Exercise 1

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git init
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "resolving conflict file"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git remote add origin https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git pull origin main --allow-unrelated-histories
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "committing change"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b div
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch -m div dev
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin -u dev
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b test
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout dev
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch -d test
# Bundle 1 - Exercise 2

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash push -m "incomplete about.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash push -m "incompelete team.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash push -m "incomplete home.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash pop "stash@{2}"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash pop "stash@{0}"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "new file changed"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash pop "stash@{0}"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "last file "
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin dev
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash push -m "new change on team.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git stash pop "stash@{0}"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git reset --hard
# Bundle 2 - Exercise 1

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/bundle-2
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\services.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "file: services.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/bundle-2
# Bundle 2 - Exercise 2

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add index.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "file for all information"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/service-redesign
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\services.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat : new line added"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin  ft/service-redesign
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add services.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "looking conflict and resolving it"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout ft/service-redesign
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git merge main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\services.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "resolved merge conflict with main"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin ft/service-redesign
# Bundle 3 - Exercise 1

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/team-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add team.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat: changes on team.html"
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/team-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/contact-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout ft/team-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\README.md
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m ""

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
* ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git log
commit 3b7c96cda8beb236d5f94422a105e37ee914aff0 (HEAD -> ft/team-page, origin/ft/team-page)
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 16:04:33 2025 +0200

    feat: changes on team.html

commit a6b67aa9f22d6865feb45ece109ff5aa4cd0ba22 (origin/ft/service-redesign, ft/service-redesign)
Merge: fb97791 ca1b815
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 15:51:00 2025 +0200

    resolved merge conflict with main

commit ca1b8152c82411c486002206f272206b62736c7a (ft/contact-page)
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 15:42:24 2025 +0200

    looking conflict and resolving it

commit fb977913c7588641efddd470ebc3003eab111c12
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 15:31:33 2025 +0200

    feat : new line added

commit 5aa49f0ab981376b6688ae9c64941205211f63d1
Merge: e0d8f81 de70b9c
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 15:25:13 2025 +0200

    Merge pull request #1 from didier-bazayesu/ft/bundle-2

    File Added

commit e0d8f81af044c0e31ee669115ff4b9934bb85f00
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 14:50:00 2025 +0200

    file for all information

commit de70b9c80a601713f0ca39ce83ea72a00969e554 (origin/ft/bundle-2, ft/bundle-2)
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 14:39:30 2025 +0200

    file: services.html

commit 337d8c4f5f5de1b16041cc4889990c92adb1e749
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 13:15:27 2025 +0200

    last file

commit 789a9f58cba39cd6b9c7a647806719d060735210
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 13:12:55 2025 +0200

    new file changed

commit 96f2ef6df79669104530ddb8f19dbf028573983a (origin/dev, dev)
Merge: 529f6f8 bc75107
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 12:06:30 2025 +0200

    committing change

commit 529f6f82e74a3104a76d202dc2207cc4037a078b
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 11:51:07 2025 +0200

    resolving conflict file

commit bc75107f1d9fc89510910a5566408b16d353516a
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 10:12:55 2025 +0200

    Initial commit
...skipping...

                   SUMMARY OF LESS COMMANDS

      Commands marked with * may be preceded by a number, N.
      Notes in parentheses indicate the behavior if N is given.
      A key preceded by a caret indicates the Ctrl key; thus ^K is ctrl-K.

  h  H                 Display this help.
  q  :q  Q  :Q  ZZ     Exit.
 ---------------------------------------------------------------------------

                           MOVING

  e  ^E  j  ^N  CR  *  Forward  one line   (or N lines).
  y  ^Y  k  ^K  ^P  *  Backward one line   (or N lines).
  ESC-j             *  Forward  one file line (or N file lines).
  ESC-k             *  Backward one file line (or N file lines).
  f  ^F  ^V  SPACE  *  Forward  one window (or N lines).
  b  ^B  ESC-v      *  Backward one window (or N lines).
  z                 *  Forward  one window (and set window to N).
  w                 *  Backward one window (and set window to N).
  ESC-SPACE         *  Forward  one window, but don't stop at end-of-file.
  ESC-b             *  Backward one window, but don't stop at beginning-of-file.
  d  ^D             *  Forward  one half-window (and set half-window to N).
  u  ^U             *  Backward one half-window (and set half-window to N).
  ESC-)  RightArrow *  Right one half screen width (or N positions).
  ESC-(  LeftArrow  *  Left  one half screen width (or N positions).
  ESC-}  ^RightArrow   Right to last column displayed.
  ESC-{  ^LeftArrow    Left  to first column.
  F                    Forward forever; like "tail -f".
  ESC-F                Like F but stop when search pattern is found.
  r  ^R  ^L            Repaint screen.
  R                    Repaint screen, discarding buffered input.
        ---------------------------------------------------
        Default "window" is the screen height.
        Default "half-window" is half of the screen height.
 ---------------------------------------------------------------------------

                          SEARCHING

  /pattern          *  Search forward for (N-th) matching line.
  ?pattern          *  Search backward for (N-th) matching line.
  n                 *  Repeat previous search (for N-th occurrence).
  N                 *  Repeat previous search in reverse direction.
  ESC-n             *  Repeat previous search, spanning files.
  ESC-N             *  Repeat previous search, reverse dir. & spanning files.
  ^O^N  ^On         *  Search forward for (N-th) OSC8 hyperlink.
  ^O^P  ^Op         *  Search backward for (N-th) OSC8 hyperlink.
  ^O^L  ^Ol            Jump to the currently selected OSC8 hyperlink.
  ESC-u                Undo (toggle) search highlighting.
  ESC-U                Clear search highlighting.
  &pattern          *  Display only matching lines.
        ---------------------------------------------------
                Search is case-sensitive unless changed with -i or -I.
        A search pattern may begin with one or more of:
        ^N or !  Search for NON-matching lines.
        ^E or *  Search multiple files (pass thru END OF FILE).
        ^F or @  Start search at FIRST file (for /) or last file (for ?).
        ^K       Highlight matches, but don't move (KEEP position).
        ^R       Don't use REGULAR EXPRESSIONS.
        ^S n     Search for match in n-th parenthesized subpattern.
        ^W       WRAP search if no match found.
        ^L       Enter next character literally into pattern.
 ---------------------------------------------------------------------------

                           JUMPING

  g  <  ESC-<       *  Go to first line in file (or line N).
  G  >  ESC->       *  Go to last line in file (or line N).
  p  %              *  Go to beginning of file (or N percent into file).
  t                 *  Go to the (N-th) next tag.
  T                 *  Go to the (N-th) previous tag.
  {  (  [           *  Find close bracket } ) ].
  }  )  ]           *  Find open bracket { ( [.
  ESC-^F <c1> <c2>  *  Find close bracket <c2>.
  ESC-^B <c1> <c2>  *  Find open bracket <c1>.
        ---------------------------------------------------
        Each "find close bracket" command goes forward to the close bracket
          matching the (N-th) open bracket in the top line.
        Each "find open bracket" command goes backward to the open bracket
          matching the (N-th) close bracket in the bottom line.

  m<letter>            Mark the current top line with <letter>.
  M<letter>            Mark the current bottom line with <letter>.
  '<letter>            Go to a previously marked position.
  ''                   Go to the previous position.
  ^X^X                 Same as '.
  ESC-m<letter>        Clear a mark.
        ---------------------------------------------------
        A mark is any upper-case or lower-case letter.
        Certain marks are predefined:
             ^  means  beginning of the file
             $  means  end of the file
 ---------------------------------------------------------------------------

                        CHANGING FILES

  :e [file]            Examine a new file.
  ^X^V                 Same as :e.
  :n                *  Examine the (N-th) next file from the command line.
  :p                *  Examine the (N-th) previous file from the command line.
  :x                *  Examine the first (or N-th) file from the command line.
  ^O^O                 Open the currently selected OSC8 hyperlink.
  :d                   Delete the current file from the command line list.
  =  ^G  :f            Print current file name.
 ---------------------------------------------------------------------------

                    MISCELLANEOUS COMMANDS

  -<flag>              Toggle a command line option [see OPTIONS below].
  --<name>             Toggle a command line option, by name.
  _<flag>              Display the setting of a command line option.
  __<name>             Display the setting of an option, by name.
  +cmd                 Execute the less cmd each time a new file is examined.

  !command             Execute the shell command with $SHELL.
  #command             Execute the shell command, expanded like a prompt.
  |Xcommand            Pipe file between current pos & mark X to shell command.
  s file               Save input to a file.
  v                    Edit the current file with $VISUAL or $EDITOR.
  V                    Print version number of "less".
 ---------------------------------------------------------------------------

                           OPTIONS

        Most options may be changed either on the command line,
        or from within less by using the - or -- command.
        Options may be given in one of two forms: either a single
        character preceded by a -, or a name preceded by --.

  -?  ........  --help
                  Display help (from command line).
  -a  ........  --search-skip-screen
                  Search skips current screen.
  -A  ........  --SEARCH-SKIP-SCREEN
                  Search starts just after target line.
  -b [N]  ....  --buffers=[N]
                  Number of buffers.
  -B  ........  --auto-buffers
                  Don't automatically allocate buffers for pipes.
  -c  ........  --clear-screen
                  Repaint by clearing rather than scrolling.
  -d  ........  --dumb
                  Dumb terminal.
  -D xcolor  .  --color=xcolor
                  Set screen colors.
  -e  -E  ....  --quit-at-eof  --QUIT-AT-EOF
                  Quit at end of file.
  -f  ........  --force
                  Force open non-regular files.
  -F  ........  --quit-if-one-screen
                  Quit if entire file fits on first screen.
  -g  ........  --hilite-search
                  Highlight only last match for searches.
  -G  ........  --HILITE-SEARCH
                  Don't highlight any matches for searches.
  -h [N]  ....  --max-back-scroll=[N]
                  Backward scroll limit.
  -i  ........  --ignore-case
                  Ignore case in searches that do not contain uppercase.
  -I  ........  --IGNORE-CASE
                  Ignore case in all searches.
  -j [N]  ....  --jump-target=[N]
                  Screen position of target lines.
  -J  ........  --status-column
                  Display a status column at left edge of screen.
  -k file  ...  --lesskey-file=file
                  Use a compiled lesskey file.
  -K  ........  --quit-on-intr
                  Exit less in response to ctrl-C.
  -L  ........  --no-lessopen
                  Ignore the LESSOPEN environment variable.
  -m  -M  ....  --long-prompt  --LONG-PROMPT
                  Set prompt style.
  -n .........  --line-numbers
                  Suppress line numbers in prompts and messages.
  -N .........  --LINE-NUMBERS
                  Display line number at start of each line.
  -o [file] ..  --log-file=[file]
                  Copy to log file (standard input only).
  -O [file] ..  --LOG-FILE=[file]
                  Copy to log file (unconditionally overwrite).
  -p pattern .  --pattern=[pattern]
                  Start at pattern (from command line).
  -P [prompt]   --prompt=[prompt]
                  Define new prompt.
  -q  -Q  ....  --quiet  --QUIET  --silent --SILENT
                  Quiet the terminal bell.
  -r  -R  ....  --raw-control-chars  --RAW-CONTROL-CHARS
                  Output "raw" control characters.
  -s  ........  --squeeze-blank-lines
                  Squeeze multiple blank lines.
  -S  ........  --chop-long-lines
                  Chop (truncate) long lines rather than wrapping.
  -t tag  ....  --tag=[tag]
                  Find a tag.
  -T [tagsfile] --tag-file=[tagsfile]
                  Use an alternate tags file.
  -u  -U  ....  --underline-special  --UNDERLINE-SPECIAL
                  Change handling of backspaces, tabs and carriage returns.
  -V  ........  --version
                  Display the version number of "less".
  -w  ........  --hilite-unread
                  Highlight first new line after forward-screen.
  -W  ........  --HILITE-UNREAD
                  Highlight first new line after any forward movement.
  -x [N[,...]]  --tabs=[N[,...]]
                  Set tab stops.
  -X  ........  --no-init
                  Don't use termcap init/deinit strings.
  -y [N]  ....  --max-forw-scroll=[N]
                  Forward scroll limit.
  -z [N]  ....  --window=[N]
                  Set size of window.
  -" [c[c]]  .  --quotes=[c[c]]
                  Set shell quote characters.
  -~  ........  --tilde
                  Don't display tildes after end of file.
  -# [N]  ....  --shift=[N]
                  Set horizontal scroll amount (0 = one half screen width).

                --exit-follow-on-close
                  Exit F command on a pipe when writer closes pipe.
                --file-size
                  Automatically determine the size of the input file.
                --follow-name
                  The F command changes files if the input file is renamed.
                --form-feed
                  Stop scrolling when a form feed character is reached.
                --header=[L[,C[,N]]]
                  Use L lines (starting at line N) and C columns as headers.
                --incsearch
                  Search file as each pattern character is typed in.
                --intr=[C]
                  Use C instead of ^X to interrupt a read.
                --lesskey-context=text
                  Use lesskey source file contents.
                --lesskey-src=file
                  Use a lesskey source file.
                --line-num-width=[N]
                  Set the width of the -N line number field to N characters.
                --match-shift=[N]
                  Show at least N characters to the left of a search match.
                --modelines=[N]
                  Read N lines from the input file and look for vim modelines.
                --mouse
                  Enable mouse input.
                --no-edit-warn
                  Don't warn when using v command on a file opened via LESSOPEN.
                --no-keypad
                  Don't send termcap keypad init/deinit strings.
                --no-histdups
                  Remove duplicates from command history.
                --no-number-headers
                  Don't give line numbers to header lines.
                --no-paste
                  Ignore pasted input.
                --no-search-header-lines
                  Searches do not include header lines.
                --no-search-header-columns
                  Searches do not include header columns.
                --no-search-headers
                  Searches do not include header lines or columns.
                --no-vbell
                  Disable the terminal's visual bell.
                --redraw-on-quit
                  Redraw final screen when quitting.
                --rscroll=[C]
                  Set the character used to mark truncated lines.
                --save-marks
                  Retain marks across invocations of less.
                --search-options=[EFKNRW-]
                  Set default options for every search.
                --show-preproc-errors
                  Display a message if preprocessor exits with an error status.
                --proc-backspace
                  Process backspaces for bold/underline.
                --PROC-BACKSPACE
                  Treat backspaces as control characters.
                --proc-return
                  Delete carriage returns before newline.
                --PROC-RETURN
                  Treat carriage returns as control characters.
                --proc-tab
HELP -- Press RETURN for more, or q when done...skipping...
Date:   Thu Jul 17 11:51:07 2025 +0200

    resolving conflict file

commit bc75107f1d9fc89510910a5566408b16d353516a
Author: didier-bazayesu <didierbazayesu@gmail.com>
Date:   Thu Jul 17 10:12:55 2025 +0200

    Initial commit
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git log --oneline
3b7c96c (HEAD -> ft/team-page, origin/ft/team-page) feat: changes on team.html
a6b67aa (origin/ft/service-redesign, ft/service-redesign) resolved merge conflict with main
ca1b815 (ft/contact-page) looking conflict and resolving it
fb97791 feat : new line added
5aa49f0 Merge pull request #1 from didier-bazayesu/ft/bundle-2
e0d8f81 file for all information
de70b9c (origin/ft/bundle-2, ft/bundle-2) file: services.html
337d8c4 last file
789a9f5 new file changed
:
3b7c96c (HEAD -> ft/team-page, origin/ft/team-page) feat: changes on team.html
a6b67aa (origin/ft/service-redesign, ft/service-redesign) resolved merge conflict with main
ca1b815 (ft/contact-page) looking conflict and resolving it
fb97791 feat : new line added
5aa49f0 Merge pull request #1 from didier-bazayesu/fe0d8f81 file for all information
de70b9c (origin/ft/bundle-2, ft/bundle-2) file: services.html
337d8c4 last file
789a9f5 new file changed
96f2ef6 (origin/dev, dev) committing change
529f6f8 resolving conflict file
bc75107 Initial commit
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout ft/contact-page
Switched to branch 'ft/contact-page'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git cherry-pick 3b7c96c
[ft/contact-page 9e4c81a] feat: changes on team.html
 Date: Thu Jul 17 16:04:33 2025 +0200
 1 file changed, 8 insertions(+)
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add index.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat : contact page adding line in index"
[ft/contact-page 4f3a7e9] feat : contact page adding line in index
 1 file changed, 7 insertions(+), 1 deletion(-)     
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/contact-page
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 764 bytes | 382.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page     
remote:
To https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git status
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

nothing to commit, working tree clean
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b feat/faq-page
Switched to a new branch 'feat/faq-page'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add fq.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat: fq already created"
[feat/faq-page 485e812] feat: fq already created
 1 file changed, 15 insertions(+)
 create mode 100644 fq.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions>
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/fq-page
error: src refspec ft/fq-page does not match any
error: failed to push some refs to 'https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git'  
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch                   
  dev
* feat/faq-page
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/faq-page
error: src refspec ft/faq-page does not match any
error: failed to push some refs to 'https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git'
PS ^C\Users\user\Documents\Gym Git Exercise Solutions>
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git status
On branch feat/faq-page
nothing to commit, working tree clean
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/faq-page
error: src refspec ft/faq-page does not match any
error: failed to push some refs to 'https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin feat/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 445 bytes | 445.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'feat/faq-page' on GitHub by visiting:
remote:      https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions/pull/new/feat/faq-page
remote:
To https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
 * [new branch]      feat/faq-page -> feat/faq-page
branch 'feat/faq-page' set up to track 'origin/feat/faq-page'.
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch -m feat/faq-page ft/faq-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git log --oneline
3b7c96c (HEAD -> ft/team-page, origin/ft/team-page) feat: changes on team.html
a6b67aa (origin/ft/service-redesign, ft/service-redesign) resolved merge conflict with main
ca1b815 looking conflict and resolving it
fb97791 feat : new line added
5aa49f0 Merge pull request #1 from didier-bazayesu/ft/bundle-2
e0d8f81 file for all information
de70b9c (origin/ft/bundle-2, ft/bundle-2) file: services.html
337d8c4 last file
789a9f5 new file changed
96f2ef6 (origin/dev, dev) committing change
529f6f8 resolving conflict file
bc75107 Initial commit
(END)
fb97791 feat : new line added
5aa49f0 Merge pull request #1 from didier-bazayesu/ft/bundle-2
e0d8f81 file for all information
de70b9c (origin/ft/bundle-2, ft/bundle-2) file: services.html
337d8c4 last file
789a9f5 new file changed
96f2ef6 (origin/dev, dev) committing change
529f6f8 resolving conflict file
bc75107 Initial commit
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git revert 3b7c96c
[ft/team-page d7209e1] Revert "feat: changes on team.html"
 1 file changed, 8 deletions(-)
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git log --oneline
d7209e1 (HEAD -> ft/team-page) Revert "feat: changes on team.html"
3b7c96c (origin/ft/team-page) feat: changes on team.html
a6b67aa (origin/ft/service-redesign, ft/service-redesign) resolved merge conflict with main
ca1b815 looking conflict and resolving it
fb97791 feat : new line added
5aa49f0 Merge pull request #1 from didier-bazayesu/ft/bundle-2
e0d8f81 file for all information
de70b9c (origin/ft/bundle-2, ft/bundle-2) file: services.html
337d8c4 last file
789a9f5 new file changed
96f2ef6 (origin/dev, dev) committing change
529f6f8 resolving conflict file
bc75107 Initial commit
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git revert 3b7c96c
On branch ft/team-page
Your branch is ahead of 'origin/ft/team-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add team.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "undo changes in team.html"
On branch ft/team-page
Your branch is ahead of 'origin/ft/team-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch         
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
* ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 370 bytes | 370.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
   3b7c96c..d7209e1  ft/team-page -> ft/team-page
PS C:\Users\user\Documents\Gym Git Exercise Solutions> 

# Bundle 3 - Exercise 2

s> git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
  ft/team-page
* main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout ft/faq-page
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
M       README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.       
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git status
On branch main
Your branch is up to date with 'origin/main'.       

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\README.md
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "adding line for Bundle 3 q2"
[main d924bd0] adding line for Bundle 3 q2
 1 file changed, 4 insertions(+), 1 deletion(-)     
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 342 bytes | 342.00 KiB/s, done.
   132e04a..d924bd0  main -> main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout  ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
PS ^C\Users\user\Documents\Gym Git Exercise Solutions>
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git status
On branch ft/home-page-redesign
nothing to commit, working tree clean
PS C:\Users\user\Documents\Gym Git Exercise Solutions> 

git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
  ft/team-page
* main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout ft/faq-page
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
M       README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.       
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git status
On branch main
Your branch is up to date with 'origin/main'.       

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\README.md
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "adding line for Bundle 3 q2"
[main d924bd0] adding line for Bundle 3 q2
 1 file changed, 4 insertions(+), 1 deletion(-)     
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 342 bytes | 342.00 KiB/s, done.
   132e04a..d924bd0  main -> main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout  ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
PS ^C\Users\user\Documents\Gym Git Exercise Solutions>
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git status
On branch ft/home-page-redesign
nothing to commit, working tree clean
PS C:\Users\user\Documents\Gym Git Exercise Solutions> 
 *  History restored 

PS C:\Users\user\Documents\Gym Git Exercise Solutions> 
 *  History restored 

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\team.html .\README.md
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit "feat : adding change on home page"
error: pathspec 'feat : adding change on home page' did not match any file(s) known to git
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\home.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\README.md
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat: adding change on home page"
[ft/home-page-redesign e19697d] feat: adding change on home page
 2 files changed, 61 insertions(+)
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch         
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u ft/hom-page-redesign
fatal: 'ft/hom-page-redesign' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin  ft/hom-page-redesign
error: src refspec ft/hom-page-redesign does not match any
error: failed to push some refs to 'https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin  ft/home-page-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.02 KiB | 1.02 MiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
PS C:\Users\user\Documents\Gym Git Exercise Solutions> 


# Bundle 4 - exercise 1
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git status
On branch ft/home-page-redesign
Your branch is up to date with 'origin/ft/home-page-redesign'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\README.md
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat:adding new line"
[ft/home-page-redesign 790260a] feat:adding new line
 1 file changed, 4 insertions(+), 1 deletion(-)
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin ft/home-page-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 336 bytes | 336.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
   152f187..790260a  ft/home-page-redesign -> ft/home-page-redesign
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\user\Documents\Gym Git Exercise Solutions> remote
remote : The term 'remote' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the spelling of the name, or if a path 
was included, verify that the path is correct and try again.
At line:1 char:1
+ remote
+ ~~~~~~
    + CategoryInfo          : ObjectNotFound: (remote:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\Users\user\Documents\Gym Git Exercise Solutions> git remote
origin
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git remote add git-copy https://github.com/didier-bazayesu/git-clone-exercises.git
PS C:\Users\user\Documents\Gym Git Exercise Solutions> 
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git remote
git-copy
origin
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .\home.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat: adding changes on home page"
[main a956afe] feat: adding changes on home page
 1 file changed, 4 insertions(+)
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 354 bytes | 177.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
   d924bd0..a956afe  main -> main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push git-copy
Enumerating objects: 35, done.
Counting objects: 100% (35/35), done.
Delta compression using up to 16 threads
Compressing objects: 100% (31/31), done.
Writing objects: 100% (35/35), 10.99 KiB | 937.00 KiB/s, done.
Total 35 (delta 15), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (15/15), done.
To https://github.com/didier-bazayesu/git-clone-exercises.git
 * [new branch]      main -> main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2


  # Bundle 4 exercise 2

     0675ee6..356b78f  main -> main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/footer
Switched to a new branch 'ft/footer'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git add .
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "feat: first footer changes"
[ft/footer 6143a2b] feat: first footer changes
 1 file changed, 14 insertions(+)
 create mode 100644 footer.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/footer
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 454 bytes | 227.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote:
To https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.       
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/footer
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
:
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/footer
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git merge --squash ft/footer
Updating 356b78f..6143a2b
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 14 ++++++++++++++
 1 file changed, 14 insertions(+)
 create mode 100644 footer.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git commit -m "footer changes squashing"
[ft/squashing 0b8638a] footer changes squashing
 1 file changed, 14 insertions(+)
 create mode 100644 footer.html
PS C:\Users\user\Documents\Gym Git Exercise Solutions> git push -u origin ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 454 bytes | 454.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote:      https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote:
To https://github.com/didier-bazayesu/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.
PS C:\Users\user\Documents\Gym Git Exercise Solutions>



# Bundle 5 exercises 1
