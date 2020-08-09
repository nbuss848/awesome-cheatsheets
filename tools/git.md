1. Be sure you don't have files uncommitted, if not commit them before next step.

git status

2. In project-directory create public subfolder

mkdir public

3. Move files with git mv except public subfolder to avoid errors

for file in $(ls | grep -v 'public'); do git mv $file public; done;

4. Move specific files like .htaccess etc...

git mv .htaccess public/

5. Commit changes

git commit -m 'Moved files to public/'

6. That's all !

git log -M summary

[source](https://gist.github.com/ajaegers/2a8d8cbf51e49bcb17d5)