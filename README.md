# Impacta CI/CD - Gabriel de Carvalho Andrade

a) echo 01 > arquivo.txt

b) git add arquivo.txt && git status
```
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   arquivo.txt

```
c) git commit -m "git add example - arquivo.txt"

d) echo 02 > arquivo.txt

e) git diff arquivo.txt
```
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02

```

f) git add arquivo.txt && git status
```
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

```

g) git diff arquivo.txt

```
Sem retorno
```

h) echo 03 > arquivo.txt

i) git diff arquivo.txt
```
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
```

j) git restore arquivo.txt && git status

```
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

```

k) git commit -m "step k"
```
[main a570fb9] step k
 1 file changed, 1 insertion(+), 1 deletion(-)
 ```

git log

 ```
 commit a570fb9aeb40ded325d5755f0e6b80a59128615a (HEAD -> main)
Author: Gabriel Andrade <gabriel@andrade.work>
Date:   Fri Aug 9 20:15:15 2024 -0300

    step k

commit 8e4cef54f2b1622448a63db0db804b40b1ccc916
Author: Gabriel Andrade <gabriel@andrade.work>
Date:   Fri Aug 9 20:10:01 2024 -0300

    git add example - arquivo.txt

commit a25b430278378adf921ec40fb19db2ee12d6acea (origin/main)
Author: Gabriel Andrade <gabriel@andrade.work>
Date:   Fri Aug 9 20:07:17 2024 -0300

    First commit
 ```

 l) echo "*.txt" > .gitignore

 m) touch novo.txt && git status

```
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
```
