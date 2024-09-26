总共是6行 进入编辑页面可看到。选择直连模式，感谢会飞的小猪对本项目的贡献

#!url=http://script.hub/file/_start_/https://raw.githubusercontent.com/starrytrim/notes/refs/heads/main/notability.conf end_/notability.sgmodule?type=qx-rewrite&target=shadowrocket-module&del=true

#!name=notability

[Script]

notability = type=http-response, pattern=^https?:\/\/notability\.com\/(global|subscriptions), script-path=https://raw.githubusercontent.com/starrytrim/notes/refs/heads/main/notability.js, requires-body=true, max-size=-1, timeout=60

[MITM]

hostname =%APPEND% notability.com
