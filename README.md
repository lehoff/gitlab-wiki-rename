gitlab-wiki-rename
==================

Small script to automate renaming gitlab wiki pages.

1. Put gitlab-rename-page inside the GitLab wiki repository.
1. This should be the same directory where the `.git` directory is listed.
1. This script will NOT search inside subdirectories.

Use:
gitlab-rename-page some-page new-page-name

This will rename `some-page.markdown` to `new-page-name.markdown` using a `git mv`
command and it will change all links of the form `(some-page)` 
in the `.markdown` and `.md` files in your directory to `(new-page-name)`.

After that you have to add and commit the changes.


