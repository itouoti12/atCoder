## JavaのAtcoder環境をvscodeで作る

 - 拡張機能Java Extention Packをインストールする
 - F5を押すとデバッグスタートする。launch.jsonが作られる
 - そのままだとコンソール入力ができないので、launch.jsonを以下のように書き換える
 
 ```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "type": "java",
            "name": "Debug (Launch)",
            "request": "launch",
            "cwd": "${workspaceFolder}",
            "console": "integratedTerminal",
            "stopOnEntry": false,
            "mainClass": "",
            "args": ""
        }
    ]
}
 ```