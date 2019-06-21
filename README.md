# learning-javascript-01

テクノロジー（藤原）JavaScriptの練習 (1)

## Q1の回答「コメントを解除したことで、どう変化しましたか？」

【ポップアップが開いて「こんにちわ」と表記が出た。】

## Q2の回答「エラーの原因は何でしょうか？（調べてみましょう）」

【「ReferenceError：ウィンドウが定義されていません
」Nuxt.js だと SSR の影響で window とか document を使うとエラーが出る。https://note.mu/in_colors_net/n/n1a9bc57fe15d】

## Chromeデベロッパーツール：Consoleの実行結果

```
【おはよう！
index.html:56 Live reload enabled.
favicon.ico:1 Failed to load resource: the server responded with a status of 404 (Not Found)
index.html:18 おはよう！
2Navigated to http://127.0.0.1:5500/index.html
index.html:18 おはよう！
Navigated to http://127.0.0.1:5500/index.html
index.html:18 おはよう！
Navigated to http://127.0.0.1:5500/index.html
VM113 main.js:4 Good morning.
index.html:18 おはよう！
Navigated to http://127.0.0.1:5500/index.html
VM135 main.js:4 Good morning.
index.html:18 おはよう！
Navigated to http://127.0.0.1:5500/index.html
VM157 main.js:4 Good morning.
index.html:18 おはよう！
Navigated to http://127.0.0.1:5500/index.html
VM179 main.js:4 Good morning.
index.html:18 おはよう！
index.html:52 [Intervention] Blocked attempt to show a 'beforeunload' confirmation panel for a frame that never had a user gesture since its load. https://www.chromestatus.com/feature/5082396709879808
socket.onmessage @ index.html:52
Navigated to http://127.0.0.1:5500/index.html
VM201 main.js:4 Good morning.
index.html:18 おはよう！
index.html:52 [Intervention] Blocked attempt to show a 'beforeunload' confirmation panel for a frame that never had a user gesture since its load. https://www.chromestatus.com/feature/5082396709879808
socket.onmessage @ index.html:52
Navigated to http://127.0.0.1:5500/index.html
VM223 main.js:4 Good morning.
index.html:18 おはよう！
index.html:52 [Intervention] Blocked attempt to show a 'beforeunload' confirmation panel for a frame that never had a user gesture since its load. https://www.chromestatus.com/feature/5082396709879808
socket.onmessage @ index.html:52
Navigated to http://127.0.0.1:5500/index.html
VM245 main.js:4 Good morning.
index.html:18 おはよう！
index.html:52 [Intervention] Blocked attempt to show a 'beforeunload' confirmation panel for a frame that never had a user gesture since its load. https://www.chromestatus.com/feature/5082396709879808
socket.onmessage @ index.html:52
Navigated to http://127.0.0.1:5500/index.html】
```

## ターミナルの実行結果

```
【Last login: Fri Jun 14 09:53:34 on ttys000
-bash: /Users/hiraikeryuta/.bash_profile: line 10: syntax error: unexpected end of file
heichiryuudainoMacBook-Pro:~ hiraikeryuta$ ls
AT.postflight.12191	Downloads		Pictures		program
Amazon Drive		Google ドライブ		Public			ryuuryuu
Applications		IoT			VirtualBox		souko
Creative Cloud Files	Library			VirtualBox VMs		ssh
Desktop			Movies			fujiwara		移送予定
Documents		Music			kid			趣味やん
heichiryuudainoMacBook-Pro:~ hiraikeryuta$ pwd
/Users/hiraikeryuta
heichiryuudainoMacBook-Pro:~ hiraikeryuta$ cd ~/fujiwara
heichiryuudainoMacBook-Pro:fujiwara hiraikeryuta$ ls
hello-git		learning-http-message	sample-web-server	simple-web-site
heichiryuudainoMacBook-Pro:fujiwara hiraikeryuta$ git clone git@github.com:ryuuryuuryuu/learning-javascript-01.git
Cloning into 'learning-javascript-01'...
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 10 (delta 0), reused 7 (delta 0), pack-reused 0
Receiving objects: 100% (10/10), done.
heichiryuudainoMacBook-Pro:fujiwara hiraikeryuta$ ls
hello-git		learning-javascript-01	simple-web-site
learning-http-message	sample-web-server
heichiryuudainoMacBook-Pro:fujiwara hiraikeryuta$ cd learning-javascript-01/
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ code .
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js
-bash: node: command not found
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ ls
README.md	index.html	js		node-main.js
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js 
-bash: node: command not found
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ brew uninstall nodebrew
Error: No such keg: /usr/local/Cellar/nodebrew
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ brew uninstall node
Error: No such keg: /usr/local/Cellar/node
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ xcode-select --install
xcode-select: error: command line tools are already installed, use "Software Update" to install updates
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ grep nodebrew
^C
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ locate nodebrew

WARNING: The locate database (/var/db/locate.database) does not exist.
To create the database, run the following command:

  sudo launchctl load -w /System/Library/LaunchDaemons/com.apple.locate.plist

Please be aware that the database can take some time to generate; once
the database has been created, this message will no longer appear.

heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ yum nodebrew
-bash: yum: command not found
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js 
-bash: node: command not found
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ which -a node
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ cd /
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ which -a node
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ which -a -node
which: illegal option -- n
usage: which [-as] program ...
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ which -a -bash
which: illegal option -- b
usage: which [-as] program ...
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ which -a node
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ which -a python
/usr/local/bin/python
/usr/bin/python
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ which -a node
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ node -v
-bash: node: command not found
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ echo "export PATH=$HOME/.nodebrew/current/bin:$PATH" >> ~/.bashrc
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ node -v
-bash: node: command not found
heichiryuudainoMacBook-Pro:/ hiraikeryuta$  cat ~/.bash_profile

# Setting PATH for Python 3.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH
if [ -f ~/.bashrc ]; then
if [ -f ~/.bashrc ]; then
  . ~/.bashrc
fi
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ curl -L git.io/nodebrew | perl - setup
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0
  0     0    0     0    0     0      0      0 --:--:--  0:00:02 --:--:--     0
100 24634  100 24634    0     0   8293      0  0:00:02  0:00:02 --:--:--  890k
Fetching nodebrew...
Installed nodebrew in $HOME/.nodebrew

========================================
Export a path to nodebrew:

export PATH=$HOME/.nodebrew/current/bin:$PATH
========================================
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ source ~/.bashrc
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ node -v
v12.4.0
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ nodebrew
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
heichiryuudainoMacBook-Pro:/ hiraikeryuta$ cd ~/fujiwara
heichiryuudainoMacBook-Pro:fujiwara hiraikeryuta$ ls
hello-git		learning-javascript-01	simple-web-site
learning-http-message	sample-web-server
heichiryuudainoMacBook-Pro:fujiwara hiraikeryuta$ cd learning-javascript-01/
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ ls
README.md	index.html	js		node-main.js
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js 
/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js 
/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js 
/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js 
/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js 
/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js 
/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/hiraikeryuta/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ node node-main.js 
Goodmorning, Node.js!!
heichiryuudainoMacBook-Pro:learning-javascript-01 hiraikeryuta$ 
】
```

