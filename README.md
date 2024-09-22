总共是6行

#!url=http://script.hub/file/_start_/https://raw.githubusercontent.com/starrytrim/notes/refs/heads/main/notability.conf end_/notability.sgmodule?type=qx-rewrite&target=shadowrocket-module&del=true
#!name=notability

[Script]
notability = type=http-response, pattern=^https?:\/\/notability\.com\/(global|subscriptions), script-path=https://raw.githubusercontent.com/starrytrim/notes/refs/heads/main/notability.js, requires-body=true, max-size=-1, timeout=60

[MITM]
hostname =%APPEND% notability.com
