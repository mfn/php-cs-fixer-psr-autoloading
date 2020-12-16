# Using 2.16.9
```
$ ./php-cs-fixer-2.16.9.phar fix --diff --diff-format=udiff --dry-run -vv
Loaded config default from "/Users/neo/tmp/php-cs-fixer-psr-autoloading/.php_cs.dist".
Runtime: PHP 7.4.13
Using cache file ".php_cs.cache".
..
Legend: ?-unknown, I-invalid file syntax (file ignored), S-skipped (cached or empty file), .-no changes, F-fixed, E-error

Checked all files in 0.006 seconds, 12.000 MB memory used
```

# Using 2.17.1
```
$ ./php-cs-fixer-2.17.1.phar fix --diff --diff-format=udiff --dry-run -vv
Loaded config default from "/Users/neo/tmp/php-cs-fixer-psr-autoloading/.php_cs.dist".
Runtime: PHP 7.4.13
Using cache file ".php_cs.cache".
SE
Legend: ?-unknown, I-invalid file syntax (file ignored), S-skipped (cached or empty file), .-no changes, F-fixed, E-error

Checked all files in 0.004 seconds, 12.000 MB memory used

Files that were not fixed due to errors reported during linting after fixing:
   1) /Users/neo/tmp/php-cs-fixer-psr-autoloading/Test2/___file.php


        [PhpCsFixer\Linter\LintingException]
        Parse error: syntax error, unexpected '-', expecting identifier (T_STRING) on line 3.


      Applied fixers: psr4
      ---------- begin diff ----------
--- Original
+++ New
@@ -1,4 +1,4 @@
 <?php

-class NamedCompletelyDifferently {
+class -autoloading_Test2____file {
 }

      ----------- end diff -----------
```
