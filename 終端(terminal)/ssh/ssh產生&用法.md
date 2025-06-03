```shell
# 輸入以下指令，然後 enter 到底
ssh-keygen -t rsa -C "wkai2573@gmail"

# PS C:\> ssh-keygen
# Generating public/private rsa key pair.
# Enter file in which to save the key (C:\Users\admin/.ssh/id_rsa):       
# Enter passphrase (empty for no passphrase): 
# Enter same passphrase again: 
# Your identification has been saved in C:\Users\admin/.ssh/id_rsa.
# Your public key has been saved in C:\Users\admin/.ssh/id_rsa.pub.
# The key fingerprint is:
# SHA256:Tl83XQmNbugRFMvgRhniqoTek5SB/ZZFHnyXSA6h48U admin@LAPTOP-ADJQRR3U
# The key's randomart image is:
# +---[RSA 3072]----+
# |      .*o==oo.o  |
# |  o   *.B+o+.....|
# | . o o E.+.o+  ..|
# |  . = * .  o o ..|
# | . + *  S . + o .|
# |. + +  o . o . . |
# | . =    . .      |
# |    .            |
# |                 |
# +----[SHA256]-----+


# 然後到 C:\Users\admin/.ssh/ 查看產生的檔案
# 私鑰: C:\Users\admin/.ssh/id_rsa
# 公鑰: C:\Users\admin/.ssh/id_rsa.pub

# 把公鑰裡的字串全部 複製到需要公鑰的地方即可 (ex. github 或 gitlab ...)

```
