# pnpm-diff-files-examples

To reproduce the issue:

- clone the repo
- `pnpm i`
- `git status`

  Expected and observed:
  
  ```
  On branch main
  Your branch is up to date with 'origin/main'.

  nothing to commit, working tree clean
  ```
  
- `git diff-files --`

  Expected: 
  
  ```
  > git diff-files --
  # no file listed
  ```

  Observed: 

  ```
  > git diff-files --
  :100755 100755 e69de29bb2d1d6434b8b29ae775ad8c2e48c5391 0000000000000000000000000000000000000000 M	packages/one/bin/test.sh
  ```
  
