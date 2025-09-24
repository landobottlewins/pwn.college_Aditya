# An Epic Filesystem Quest
## My solve
**Flag:** `pwn.college{wPsAlWPbX6UqjBr316UtAQy06Kj.QX5IDO0wyM1gjNzEzW}`

```bash
Connected!
hacker@commands~an-epic-filesystem-quest:~$  cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
INFO  challenge  flag  lib32   media  opt   run   sys  var
bin   dev        home  lib64   mnt    proc  sbin  tmp
boot  etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ cat INFO
Congratulations, you found the clue!
The next clue is in: /usr/local/lib/python3.8/dist-packages/networkx/drawing/tests/baseline

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/local/lib/python3.8/dist-packages/networkx/drawing/tests/baseline
BLUEPRINT-TRAPPED  test_house_with_colors.png
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/local/lib/python3.8/dist-packages/networkx/drawing/tests/baseline/BLUEPRINT-TRAPPED
Congratulations, you found the clue!
The next clue is in: /usr/share/icons/hicolor/22x22/apps

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/icons/hicolor/22x22/apps
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/22x22/apps$ ls
BRIEF  firefox.png
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/22x22/apps$ cat BRIEF
Tubular find!
The next clue is in: /opt/linux/linux-5.4/tools/testing/selftests/pstore

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/22x22/apps$ cd /opt/linux/linux-5.4/tools/testing/selftests/pstore
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/testing/selftests/pstore$ ls -a
.  ..  .GIST  .gitignore  Makefile  common_tests  config  pstore_crash_test  pstore_post_reboot_tests  pstore_tests
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/testing/selftests/pstore$ cat .GIST
Tubular find!
The next clue is in: /opt/linux/linux-5.4/drivers/staging/android/ion

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
DOSSIER-TRAPPED  Kconfig  Makefile  ion.c  ion.h  ion_cma_heap.c  ion_heap.c  ion_page_pool.c  ion_system_heap.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/testing/selftests/pstore$ cat /opt/linux/linux-5.4/drivers/staging/android/ion/DOSSIER-TRAPPED
Congratulations, you found the clue!
The next clue is in: /usr/share/maxima-sage/5.42.2/share/amatrix

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/testing/selftests/pstore$ cd /usr/share/maxima-sage/5.42.2/share/amatrix
hacker@commands~an-epic-filesystem-quest:/usr/share/maxima-sage/5.42.2/share/amatrix$ ls
README  WHISPER  amatrix.dem  amatrix.lisp  amatrix.mac  rtest_amatrix.mac  rtest_wilcoxon.mac  wilcoxon.mac
hacker@commands~an-epic-filesystem-quest:/usr/share/maxima-sage/5.42.2/share/amatrix$ cat WHISPER
Lucky listing!
The next clue is in: /usr/share/help/ru/gedit

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/maxima-sage/5.42.2/share/amatrix$ cd /usr/share/help/ru/gedit
hacker@commands~an-epic-filesystem-quest:/usr/share/help/ru/gedit$ ls -a
.                               gedit-files-basic.page               gedit-plugins-external-tools.page    gedit-printing-order.page   gedit-syntax-highlighting.page
..                              gedit-full-screen.page               gedit-plugins-file-browser.page      gedit-printing-select.page  gedit-tab-groups.page
.EVIDENCE                       gedit-open-files-from-sidepane.page  gedit-plugins-insert-date-time.page  gedit-printing.page         gedit-tabs-moving.page
figures                         gedit-open-files.page                gedit-plugins-install.page           gedit-quickstart.page       gedit-tabs.page
gedit-change-color-scheme.page  gedit-open-on-server.page            gedit-plugins-modelines.page         gedit-replace.page          gedit-undo-recent-action.page
gedit-change-default-font.page  gedit-open-recent.page               gedit-plugins-pyconsole.page         gedit-save-file.page        index.page
gedit-close-file.page           gedit-plugin-guide.page              gedit-plugins-quick-open.page        gedit-search.page           legal.xml
gedit-create-new-file.page      gedit-plugins-change-case.page       gedit-plugins-snippets.page          gedit-shortcut-keys.page
gedit-edit-as-root.page         gedit-plugins-doc-stats.page         gedit-plugins-sort.page              gedit-spellcheck.page
hacker@commands~an-epic-filesystem-quest:/usr/share/help/ru/gedit$ cat .EVIDENCE
Yahaha, you found me!
The next clue is in: /usr/local/lib/python3.8/dist-packages/defusedxml
hacker@commands~an-epic-filesystem-quest:/usr/share/help/ru/gedit$ ls /usr/local/lib/python3.8/dist-packages/defusedxml
ElementTree.py  SPOILER  __init__.py  __pycache__  cElementTree.py  common.py  expatbuilder.py  expatreader.py  lxml.py  minidom.py  pulldom.py  sax.py  xmlrpc.py
hacker@commands~an-epic-filesystem-quest:/usr/share/help/ru/gedit$ cat /usr/local/lib/python3.8/dist-packages/defusedxml/SPOILER
Great sleuthing!
The next clue is in: /usr/share/doc/python3-psutil

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/help/ru/gedit$ cd /usr/share/doc/python3-psutil
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/python3-psutil$ ls -a
.  ..  .POINTER  changelog.Debian.gz  copyright
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/python3-psutil$ cat .POINTER
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{wPsAlWPbX6UqjBr316UtAQy06Kj.QX5IDO0wyM1gjNzEzW}

```

## Incorrect tangents I went on
none

## What I learned
Implemented the knowledege of `cd`, `ls`, `cat` 

## References 
None
