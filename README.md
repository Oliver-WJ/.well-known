# .well-known  深度链接是一种 intent 过滤器。应用链接是一种特殊的深度链接，基于已验证的网站网址。
深度链接
在询问用户是否app打开时，如果用户选择了“取消”，那么下次再想点击链接打开app时，将不会有反应。

当点击链接，而本地有多个app 匹配时，会弹出“应用选择弹框”，用户必须选择对应的应用才能打开app。

应用链接
直接打开匹配的应用，不会出现对话框。

相比深度链接，应用链接更加繁琐。
需要在过滤器添加 android:autoVerify=“true”。
< data> 中的 android:scheme 属性必须为 “http 或者 https”
需要配置 assetlinks.json
