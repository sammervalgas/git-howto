# Advanced Commands #



### Merge

Terminologia
|Symbol|Description|
|:-----:|:-----:|
|<|Local Changes|
|=|Separation|
|>|Remote Changes|

```bash
git merge

git mergetool --tool-help

# Free tools  kdiff3, Meld ou P4Merge
git mergetool -t [nome_do_programa] 

```
> Técnica:
>   Para evitar trabalhos com merge é altamente recomendado que sejam realizados commits pequenos (git commit) e sincronização  (git pull) frequentemente.