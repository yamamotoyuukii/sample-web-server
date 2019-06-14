# sample-web-server
テクノロジー（藤原）Node.jsによるサンプルWebサーバ

```
Last login: Fri Jun 14 09:07:43 on ttys001
You have mail.
yamamotoyuukinoMacBook-Pro:~ yamamotoyuuki$ cd ~/fujiwara
yamamotoyuukinoMacBook-Pro:fujiwara yamamotoyuuki$ git clone git@github.com:yamamotoyuukii/sample-web-server.git
Cloning into 'sample-web-server'...
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 7 (delta 1), reused 5 (delta 1), pack-reused 0
Receiving objects: 100% (7/7), done.
Resolving deltas: 100% (1/1), done.
yamamotoyuukinoMacBook-Pro:fujiwara yamamotoyuuki$ cd sample-web-server
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ code .
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ https://api.thecatapi.com/v1/images/search
-bash: https://api.thecatapi.com/v1/images/search: No such file or directory
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ GET /images/search
-bash: GET: command not found
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ curl --silent --request GET --url https://api.thecatapi.com/v1/images/search
[{"breeds":[],"id":"cmb","url":"https://cdn2.thecatapi.com/images/cmb.jpg","width":560,"height":487}]yamamotoyuukinoMacBook-Pro: --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3'
[{"breeds":[],"id":"24m","url":"https://cdn2.thecatapi.com/images/24m.jpg","width":450,"height":337},{"breeds":[],"id":"cd2","url":"https://cdn2.thecatapi.com/images/cd2.jpg","width":400,"height":470},{"breeds":[],"id":"cks","url":"https://cdn2.thecatapi.com/images/cks.jpg","width":500,"height":333}]yamamotoyuukinoMacB install jqple-web-server yamamotoyuuki$ brew 
Updating Homebrew...
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
==> New Formulae
scala@2.12                       swig@3
==> Updated Formulae
openssl ✔             go                    phpunit
pyenv ✔               godep                 procs
armadillo             graph-tool            pulumi
atlantis              gst-plugins-good      pybind11
aws-sdk-cpp           helmfile              rbspy
bitrise               hlint                 scala
braid                 imagemagick           scalariform
calicoctl             imagemagick@6         scons
certbot               jdupes                scrcpy
cfn-lint              jfrog-cli-go          serverless
chakra                jhipster              ship
circleci              joplin                sops
citus                 knot                  telegraf
composer              libev                 terraform
doctl                 librealsense          terragrunt
encfs                 libsigc++             tokei
envconsul             lmod                  topgrade
exiftool              macvim                vultr
firebase-cli          mesa                  webpack
flow                  mighttpd2             whois
fluxctl               minio                 wildfly-as
folly                 minio-mc              wtf
gibo                  nomad                 yelp-tools
glib                  opa                   you-get
glooctl               paket
gmic                  pandoc
==> Deleted Formulae
scala@2.10                       swig@3.04

==> Installing dependencies for jq: oniguruma
==> Installing jq dependency: oniguruma
==> Downloading https://homebrew.bintray.com/bottles/oniguruma-6
==> Downloading from https://akamai.bintray.com/c6/c613befafe81d
#####################                                           ###################################################             ######################################################################## 100.0%
==> Pouring oniguruma-6.9.2.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/oniguruma/6.9.2: 17 files, 1.3MB
==> Installing jq
==> Downloading https://homebrew.bintray.com/bottles/jq-1.6.moja
==> Downloading from https://akamai.bintray.com/71/71f0e76c5b22e
###########################################                     ######################################################################## 100.0%
==> Pouring jq-1.6.mojave.bottle.1.tar.gz
🍺  /usr/local/Cellar/jq/1.6: 18 files, 1MB
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' | jq
[
  {
    "breeds": [],
    "id": "20o",
    "url": "https://cdn2.thecatapi.com/images/20o.jpg",
    "width": 500,
    "height": 500
  },
  {
    "breeds": [],
    "id": "ck5",
    "url": "https://cdn2.thecatapi.com/images/ck5.jpg",
    "width": 1024,
    "height": 768
  },
  {
    "breeds": [],
    "categories": [
      {
        "id": 14,
        "name": "sinks"
      }
    ],
    "id": "MTc5NjQ3NQ",
    "url": "https://cdn2.thecatapi.com/images/MTc5NjQ3NQ.jpg",
    "width": 960,
    "height": 720
  }
]
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' > thecat.json
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' > thecat.json
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ cat ~/.bash_profile
# added by Anaconda3 2019.03 installer
# >>> conda init >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$(CONDA_REPORT_ERRORS=false '/Users/yamamotoyuuki/anaconda3/bin/conda' shell.bash hook 2> /dev/null)"
if [ $? -eq 0 ]; then
    \eval "$__conda_setup"
else
    if [ -f "/Users/yamamotoyuuki/anaconda3/etc/profile.d/conda.sh" ]; then
        . "/Users/yamamotoyuuki/anaconda3/etc/profile.d/conda.sh"
        CONDA_CHANGEPS1=false conda activate base
    else
        \export PATH="/Users/yamamotoyuuki/anaconda3/bin:$PATH"
    fi
fi
unset __conda_setup
# <<< conda init <<<

# Setting PATH for Python 3.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH
if [ -f ~/.bashrc ]; then
  . ~/.bashrc
fi
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ clear

yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ cat ~/.bash_profile
# added by Anaconda3 2019.03 installer
# >>> conda init >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$(CONDA_REPORT_ERRORS=false '/Users/yamamotoyuuki/anaconda3/bin/conda' shell.bash hook 2> /dev/null)"
if [ $? -eq 0 ]; then
    \eval "$__conda_setup"
else
    if [ -f "/Users/yamamotoyuuki/anaconda3/etc/profile.d/conda.sh" ]; then
        . "/Users/yamamotoyuuki/anaconda3/etc/profile.d/conda.sh"
        CONDA_CHANGEPS1=false conda activate base
    else
        \export PATH="/Users/yamamotoyuuki/anaconda3/bin:$PATH"
    fi
fi
unset __conda_setup
# <<< conda init <<<

# Setting PATH for Python 3.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH
if [ -f ~/.bashrc ]; then
  . ~/.bashrc
fi
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ suddo vi .bash_profile
-bash: suddo: command not found
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ sudo vi .bash_profile
Password:
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ cat ~/.bash_profile
# added by Anaconda3 2019.03 installer
# >>> conda init >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$(CONDA_REPORT_ERRORS=false '/Users/yamamotoyuuki/anaconda3/bin/conda' shell.bash hook 2> /dev/null)"
if [ $? -eq 0 ]; then
    \eval "$__conda_setup"
else
    if [ -f "/Users/yamamotoyuuki/anaconda3/etc/profile.d/conda.sh" ]; then
        . "/Users/yamamotoyuuki/anaconda3/etc/profile.d/conda.sh"
        CONDA_CHANGEPS1=false conda activate base
    else
        \export PATH="/Users/yamamotoyuuki/anaconda3/bin:$PATH"
    fi
fi
unset __conda_setup
# <<< conda init <<<

# Setting PATH for Python 3.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH
if [ -f ~/.bashrc ]; then
  . ~/.bashrc
fi
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ sudo vi .bash_profile
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ sudo vi ~/.bash_profile
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ cat ~/.bash_profile
# added by Anaconda3 2019.03 installer
# >>> conda init >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$(CONDA_REPORT_ERRORS=false '/Users/yamamotoyuuki/anaconda3/bin/conda' shell.bash hook 2> /dev/null)"
if [ $? -eq 0 ]; then
    \eval "$__conda_setup"
else
    if [ -f "/Users/yamamotoyuuki/anaconda3/etc/profile.d/conda.sh" ]; then
        . "/Users/yamamotoyuuki/anaconda3/etc/profile.d/conda.sh"
        CONDA_CHANGEPS1=false conda activate base
    else
        \export PATH="/Users/yamamotoyuuki/anaconda3/bin:$PATH"
    fi
fi
unset __conda_setup
# <<< conda init <<<

# Setting PATH for Python 3.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH
if [ -f ~/.bashrc ]; then
  . source /.bashrc
fi
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ curl -L git.io/nodebrew | perl - setup
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:--   0     0    0     0    0     0      0      0 --:--:-- --:--:--   0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
  0     0    0     0    0     0      0      0 --:--:--  0:00:01   0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0
  0     0    0     0    0     0      0      0 --:--:--  0:00:02   0     0    0     0    0     0      0      0 --:--:--  0:00:02 --:--:--     0
100 24634  100 24634    0     0   8418      0  0:00:02  0:00:02 --:--:--  8418
Fetching nodebrew...
Installed nodebrew in $HOME/.nodebrew

========================================
Export a path to nodebrew:

export PATH=$HOME/.nodebrew/current/bin:$PATH
========================================
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ export PATH=$HOME/.nodebrew/current/bin:$PATH >> ~/.bashrc
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ source ~/.bashrc
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ nodebrew
nodebrew 1.0.1

Usage:
    nodebrew help                         Show this message
    nodebrew install <version>            Download and install <version> (from binary)
    nodebrew compile <version>            Download and install <version> (from source)
    nodebrew install-binary <version>     Alias of `install` (For backward compatibility)
    nodebrew uninstall <version>          Uninstall <version>
    nodebrew use <version>                Use <version>
    nodebrew list                         List installed versions
    nodebrew ls                           Alias for `list`
    nodebrew ls-remote                    List remote versions
    nodebrew ls-all                       List remote and installed versions
    nodebrew alias <key> <value>          Set alias
    nodebrew unalias <key>                Remove alias
    nodebrew clean <version> | all        Remove source file
    nodebrew selfupdate                   Update nodebrew
    nodebrew migrate-package <version>    Install global NPM packages contained in <version> to current version
    nodebrew exec <version> -- <command>  Execute <command> using specified <version>

Example:
    # install
    nodebrew install v8.9.4

    # use a specific version number
    nodebrew use v8.9.4
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ nodebrew install-binary latest
v12.4.0 is already installed
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ node -v
v12.4.0
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ mkdir mywebbapi
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ cd mywebpi
-bash: cd: mywebpi: No such file or directory
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ cd mywebbai
-bash: cd: mywebbai: No such file or directory
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ cd mywebbpi
-bash: cd: mywebbpi: No such file or directory
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ cd mywebbpi
-bash: cd: mywebbpi: No such file or directory
yamamotoyuukinoMacBook-Pro:sample-web-server yamamotoyuuki$ cd mywebbapi
yamamotoyuukinoMacBook-Pro:mywebbapi yamamotoyuuki$ npm init
This utility will walk you through creating a package.json file.
It only covers the most common items, and tries to guess sensible defaults.

See `npm help json` for definitive documentation on these fields
and exactly what they do.

Use `npm install <pkg>` afterwards to install a package and
save it as a dependency in the package.json file.

Press ^C at any time to quit.
package name: (mywebbapi) 
version: (1.0.0) 
description: 
entry point: (index.js) 
test command: 
git repository: 
keywords: 
author: 
license: (ISC) 
About to write to /Users/yamamotoyuuki/fujiwara/sample-web-server/mywebbapi/package.json:

{
  "name": "mywebbapi",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC"
}


Is this OK? (yes) 
yamamotoyuukinoMacBook-Pro:mywebbapi yamamotoyuuki$ npm install --save express
npm notice created a lockfile as package-lock.json. You should commit this file.
npm WARN mywebbapi@1.0.0 No description
npm WARN mywebbapi@1.0.0 No repository field.

+ express@4.17.1
added 50 packages from 37 contributors and audited 126 packages in 10.181s
found 0 vulnerabilities

yamamotoyuukinoMacBook-Pro:mywebbapi yamamotoyuuki$ vi index.js
yamamotoyuukinoMacBook-Pro:mywebbapi yamamotoyuuki$ node -v
v12.4.0
yamamotoyuukinoMacBook-Pro:mywebbapi yamamotoyuuki$ node index.js
Listening on port 3000
^C
yamamotoyuukinoMacBook-Pro:mywebbapi yamamotoyuuki$ vi index.js
yamamotoyuukinoMacBook-Pro:mywebbapi yamamotoyuuki$ node index.js
Listening on port 3000
^C
yamamotoyuukinoMacBook-Pro:mywebbapi yamamotoyuuki$ 
```
