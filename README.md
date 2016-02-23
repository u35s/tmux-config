tmux配置
====
此项目为[vic2016]的tmux配置及tmux的常用操作方法

基本的配置
____
* 更换`<prefix>`为`C-a`
* 更换复制方式为vi模式
* 绑定快捷键R重新加载配置

tmux基本的使用手法
____
* 把当前屏幕分割为左右两个面板 `C-a %`
* 把当前屏幕分割为上下两个面板 `C-a "`
* 退出当前面板 `C-a d`
* 调整当前面板大小 `C-a +方向键`

tmux会话操作
____
* 创建并指定会话名字 `tmux new -s $session_name`
* 删除指定会话名字 `tmux kill-session -t $session_name`
* 临时退出会话 `C-a d`
* 列出会话 `tmux ls`
* 进入已存在的会话 `tmux a -t $session_name`

tmux注意事项
____
* tmux会记录你的工作状态,尝试不用某个回话应主动关闭,关闭全部指令`tmux kill-server`
