# 临时内存

- 仿造内存$0601相关命令jsr $c759的一个变形命令
- 开辟内存$5c30-$5cb0 执行命令是jsr $5f80
- 可以将后面的指令复制到内存中执行
- 避免切页冲突