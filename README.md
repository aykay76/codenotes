# codenotes

```
[alan@archlinux tmp]$ git clone https://github.com/hashicorp/terraform
Cloning into 'terraform'...
remote: Enumerating objects: 225, done.
remote: Counting objects: 100% (225/225), done.
remote: Compressing objects: 100% (147/147), done.
remote: Total 215993 (delta 85), reused 151 (delta 55), pack-reused 215768
Receiving objects: 100% (215993/215993), 166.38 MiB | 4.36 MiB/s, done.
Resolving deltas: 100% (131191/131191), done.
[alan@archlinux tmp]$ du -d1 -h
248M	./terraform
248M	.
[alan@archlinux tmp]$ rm -rf terraform
[alan@archlinux tmp]$ git clone https://github.com/hashicorp/terraform --depth 1
Cloning into 'terraform'...
remote: Enumerating objects: 8100, done.
remote: Counting objects: 100% (8100/8100), done.
remote: Compressing objects: 100% (6438/6438), done.
remote: Total 8100 (delta 835), reused 5546 (delta 560), pack-reused 0
Receiving objects: 100% (8100/8100), 10.56 MiB | 2.74 MiB/s, done.
Resolving deltas: 100% (835/835), done.
[alan@archlinux tmp]$ du -d1 -h
87M	./terraform
87M	.
```
