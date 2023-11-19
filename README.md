# HaohahaPPT

本项目基于 [jyyslide-md](https://github.com/zweix123/jyyslide-md#install) 构建自动化脚本，实现一键安装，直接上手使用。

## Install

- 首先打开 `scripts/` 文件夹内的四个 `.txt` 内容，分别需要你设置:

   - `echo "REMOTE_NAME" > remote_name.txt` : `REMOTE_NAME` 是你想要设置的远程仓库名

   - `echo "GITHUB_REMOTE" > github_remote.txt` : `GITHUB_REMOTE` 是你在 Github 上新建仓库的 ssh 地址

   - `echo "USER_EMAIL" > user_email.txt` : `USER_EMAIL` 是你想要设置邮箱地址

   - `echo "USER_NAME" > user_name.txt` : `USER_NAME` 是你想要设置的用户名

然后执行：

```bash
./scripts/install.sh [YOUR_SHELL_NAME]
```

## 使用教程

- `pptnew [DOC_NAME]` 新建一个名为 `DOC_NAME` 的 markdown 文档，并直接用 `vim` 打开进行编辑

- `pptgen [DOC_NAME]` 基于名为 `DOC_NAME` 的 markdown 文档生成名为 `DOC_NAME` 的网页PPT

- `pptopen [DOC_NAME]` 打开已建立过 名为 `DOC_NAME` 的文档，进行编辑内容


## Bugs

- 目前多次执行 `pptgen` 会重复添加文档链接到 `README.md`，后续打补丁时将采用替换方案。
