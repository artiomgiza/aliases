# aliases

#### Install:

```
curl -o ~/install_aliases  https://raw.githubusercontent.com/artiomgiza/aliases/master/install_script
chmod 777 ~/install_aliases
~/install_aliases
source ~/.aliases
rm ~/install_aliases
```

#### What is "alias"
In current context we can refer to alias as to _short shortcut to long terminal comand_ ([wiki](https://en.wikipedia.org/wiki/Alias_(command)))

#### Examples:
* `alias de="dep ensure -v"` 
  * Instead of running `dep ensure -v` you might run `de`

* `alias init="redis-server &; pg_ctl -D /usr/local/var/postgres start &; mysql.server start &;"`
  * Instead of starting _redis_, _posgress_ and _mysql_ by 3 separate commnands you might use simple _init_
 
#### More details:
This tool helps to add kind of aliases infrastructure. 
- download the initial aliases file
- add `~/.aliases` file that will store user defined aliases (with some default aliases)
- load aliases from `~/.aliases` file 
- add load aliases from `~/.aliases` file command to `bashrc` and `zshrc` to load aliases each time new terminal is opened

