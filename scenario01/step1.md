
### Single line code blocks can be copied by default
`copy me`

### It can also be disabled
`copying disabled`{{}}

### ディレクトリ内のファイルシステムを一覧表示します。
`ls -lah`{{exec}}

### 10秒感スリープします。Ctrl+cで中断できます。
次のコマンドを実行すると開始します:
`sleep 10s`{{exec}}

こちらをクリックするとスリープ中でも中断して、whoami(現在実行中のユーザー名を表示)を実行します:
`whoami`{{exec interrupt}}

### 以下は2つのコードを連続実行します。
```
uname -r
pwd
```{{copy}}

### Execute multiline code block

```
uname -r
pwd
```{{exec}}


### Execute multiline code block with Ctrl+c
Run a blocking command:
`sleep 1d`{{exec}}

End it and run others:
```
uname -r
whoami
```{{exec interrupt}}
