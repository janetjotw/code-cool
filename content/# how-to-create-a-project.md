# how-to-create-a-project

## Install Hugo

`janetjose@Janets-MBP-2 ~ % brew install hugo`

`janetjose@Janets-MBP-2 ~ % hugo version`

hugo v0.138.0+extended+withdeploy darwin/arm64 BuildDate=2024-11-06T11:22:34Z VendorInfo=brew

`janetjose@Janets-MBP-2 ~ % pwd`

/Users/janetjose

`janetjose@Janets-MBP-2 ~ % mkdir learnhugo`

`janetjose@Janets-MBP-2 ~ % pwd`

/Users/janetjose

`janetjose@Janets-MBP-2 ~ % hugo new site docs-as-code`

Congratulations! Your new Hugo site was created in /Users/janetjose/docs-as-code.

Just a few more steps...

1. Change the current directory to /Users/janetjose/docs-as-code.

2. Create or install a theme:

   - Create a new theme with the command "hugo new theme <THEMENAME>"

   - Or, install a theme from https://themes.gohugo.io/

3. Edit hugo.toml, setting the "theme" property to the theme name.

4. Create new content with the command "hugo new content <SECTIONNAME>/<FILENAME>.<FORMAT>".

5. Start the embedded web server with the command "hugo server --buildDrafts".

See documentation at https://gohugo.io/.

`janetjose@Janets-MBP-2 ~ % cd docs-as-code`

`janetjose@Janets-MBP-2 docs-as-code % ls`

archetypes	content		hugo.toml	layouts		themes

assets		data		i18n		static

`janetjose@Janets-MBP-2 docs-as-code % ls -A`

archetypes	content		hugo.toml	layouts		themes

assets		data		i18n		static

`janetjose@Janets-MBP-2 docs-as-code % git init`

hint: Using 'master' as the name for the initial branch. This default branch name

hint: is subject to change. To configure the initial branch name to use in all

hint: of your new repositories, which will suppress this warning, call:

hint: 

hint: 	git config --global init.defaultBranch <name>

hint: 

hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and

hint: 'development'. The just-created branch can be renamed via this command:

hint: 

hint: 	git branch -m <name>

Initialized empty Git repository in /Users/janetjose/docs-as-code/.git/

`janetjose@Janets-MBP-2 docs-as-code % pwd`

/Users/janetjose/docs-as-code

janetjose@Janets-MBP-2 docs-as-code % cd..

zsh: command not found: cd..

janetjose@Janets-MBP-2 docs-as-code % cd ..

janetjose@Janets-MBP-2 ~ % pwd

/Users/janetjose


`janetjose@Janets-MBP-2 ~ % cd docs-as-code`

`janetjose@Janets-MBP-2 docs-as-code % cat hugo.toml`

```
baseURL = 'https://example.org/'

languageCode = 'en-us'

title = 'My New Hugo Site'
```

`janetjose@Janets-MBP-2 docs-as-code % nano hugo.toml`

janetjose@Janets-MBP-2 docs-as-code % ls -A

.git		assets		data		i18n		static

archetypes	content		hugo.toml	layouts		themes

janetjose@Janets-MBP-2 docs-as-code % cd themes

janetjose@Janets-MBP-2 themes % ls -A

janetjose@Janets-MBP-2 themes % cd ..

`janetjose@Janets-MBP-2 docs-as-code % hugo mod init example.com`

go: creating new go.mod: module example.com

hugo: to add module requirements and sums:

	hugo mod tidy

janetjose@Janets-MBP-2 docs-as-code % git submodule add --depth 1 https://github.com/janettech/hugo-theme-relearn.git themes/hugo-theme-relearn

## Clone repo

`janetjose@Janets-MBP-2 do-docs-as-code % git clone https://github.com/janetjotw/code-cool.git`

Cloning into 'code-cool'...

remote: Enumerating objects: 3, done.

remote: Counting objects: 100% (3/3), done.

remote: Compressing objects: 100% (2/2), done.

remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)

Receiving objects: 100% (3/3), done.

`janetjose@Janets-MBP-2 do-docs-as-code % ls`

code-cool

`janetjose@Janets-MBP-2 do-docs-as-code % mkdir content`

`janetjose@Janets-MBP-2 do-docs-as-code % cd content

`janetjose@Janets-MBP-2 content % ls`

janetjose@Janets-MBP-2 content % ls

janetjose@Janets-MBP-2 content % ls -A

janetjose@Janets-MBP-2 content % pwd

/Users/janetjose/do-docs-as-code/content

`janetjose@Janets-MBP-2 content % ls`

# how-to-create-a-project.md	prerequisites.md

_index.md			reference-list.md

janetjose@Janets-MBP-2 content % cd ..

janetjose@Janets-MBP-2 do-docs-as-code % cd ..

janetjose@Janets-MBP-2 ~ % pwd

/Users/janetjose

janetjose@Janets-MBP-2 ~ % cd do-docs-as-code 

janetjose@Janets-MBP-2 do-docs-as-code % ls

code-cool	content

janetjose@Janets-MBP-2 do-docs-as-code % cd code-cool

janetjose@Janets-MBP-2 code-cool % ls

README.md

janetjose@Janets-MBP-2 code-cool % ls

README.md

janetjose@Janets-MBP-2 code-cool % cd ..

janetjose@Janets-MBP-2 do-docs-as-code % ls -A

code-cool	content

janetjose@Janets-MBP-2 do-docs-as-code % ls

code-cool

janetjose@Janets-MBP-2 do-docs-as-code % cd code-cool

`janetjose@Janets-MBP-2 code-cool % ls`

README.md	content

`janetjose@Janets-MBP-2 code-cool % git checkout -b new-branch-jose`

Switched to a new branch 'new-branch-jose'

`janetjose@Janets-MBP-2 code-cool % git add .`

`janetjose@Janets-MBP-2 code-cool % git commit -a -m "Adding new set of files"`

[new-branch-jose 8535541] Adding new set of files

 4 files changed, 8 insertions(+)

 create mode 100644 content/# how-to-create-a-project.md

 create mode 100644 content/_index.md

 create mode 100644 content/prerequisites.md

 create mode 100644 content/reference-list.md

## Git push to remote repo failed

`janetjose@Janets-MBP-2 code-cool % git push new-branch-jose`

fatal: 'new-branch-jose' does not appear to be a git repository

fatal: Could not read from remote repository.

Please make sure you have the correct access rights

and the repository exists.

## Steps to add ssh

### Start ssh agent

janetjose@Janets-MBP-2 code-cool % eval `ssh-agent -s`

Agent pid 70808

janetjose@Janets-MBP-2 code-cool % git push new-branch-jose

fatal: 'new-branch-jose' does not appear to be a git repository

fatal: Could not read from remote repository.

Please make sure you have the correct access rights

and the repository exists.

`janetjose@Janets-MBP-2 code-cool % open .git/config`

`janetjose@Janets-MBP-2 code-cool % git push - u origin master`

error: src refspec u does not match any

error: src refspec master does not match any

error: failed to push some refs to '-'

`janetjose@Janets-MBP-2 code-cool % ssh -vvv git@github.com`

`janetjose@Janets-MBP-2 code-cool % git push new-branch-jose`

fatal: 'new-branch-jose' does not appear to be a git repository

fatal: Could not read from remote repository.

Please make sure you have the correct access rights

and the repository exists.

`janetjose@Janets-MBP-2 code-cool % git remote add origin https://github.com/janetjotw/code-cool.git`

error: remote origin already exists.

`janetjose@Janets-MBP-2 code-cool % git remote -v`

origin	https://github.com/janetjotw/code-cool.git (fetch)

origin	https://github.com/janetjotw/code-cool.git (push)

`janetjose@Janets-MBP-2 code-cool % git push --set-upstream origin new-branch-jose`

Username for 'https://github.com': janetjotw

Password for 'https://janetjotw@github.com': 

remote: Support for password authentication was removed on August 13, 2021.

remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.

fatal: Authentication failed for 'https://github.com/janetjotw/code-cool.git/'

janetjose@Janets-MBP-2 code-cool % git push --set-upstream origin new-branch-jose

Username for 'https://github.com': janetjotw

Password for 'https://janetjotw@github.com': 

remote: Permission to janetjotw/code-cool.git denied to janetjotw.

fatal: unable to access 'https://github.com/janetjotw/code-cool.git/': The requested URL returned error: 403

`janetjose@Janets-MBP-2 code-cool % git push --set-upstream origin new-branch-jose`

Username for 'https://github.com': janetjotw

Password for 'https://janetjotw@github.com': 

remote: Permission to janetjotw/code-cool.git denied to janetjotw.

fatal: unable to access 'https://github.com/janetjotw/code-cool.git/': The requested URL returned error: 403

### Edit Git Config file

`janetjose@Janets-MBP-2 code-cool % ./git/config`

zsh: no such file or directory: ./git/config

janetjose@Janets-MBP-2 code-cool % open ./git/config

The file /Users/janetjose/do-docs-as-code/code-cool/git/config does not exist.

`janetjose@Janets-MBP-2 code-cool % open .git/config `      

### Paste the Personal Access Token into the “Password” field when you authenticate via the command line.

`janetjose@Janets-MBP-2 code-cool % git remote set-url origin https://janetjotw@github.com/janetjotw/code-cool.git`

`janetjose@Janets-MBP-2 code-cool % git push --set-upstream origin new-branch-jose`

Password for 'https://janetjotw@github.com': 

Enumerating objects: 8, done.

Counting objects: 100% (8/8), done.

Delta compression using up to 8 threads

Compressing objects: 100% (3/3), done.

Writing objects: 100% (7/7), 593 bytes | 593.00 KiB/s, done.

Total 7 (delta 0), reused 0 (delta 0), pack-reused 0

remote: 

remote: Create a pull request for 'new-branch-jose' on GitHub by visiting:

remote:      https://github.com/janetjotw/code-cool/pull/new/new-branch-jose

remote: 

To https://github.com/janetjotw/code-cool.git

 * [new branch]      new-branch-jose -> new-branch-jose

Branch 'new-branch-jose' set up to track remote branch 'new-branch-jose' from 'origin'.

janetjose@Janets-MBP-2 code-cool % 



