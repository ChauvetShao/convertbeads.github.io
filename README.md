# 拼豆工作台

Chauvet 的个人静态拼豆工具，无依赖、无构建步骤。清单只在浏览器内处理，不上传到服务器。

网站：https://chauvetshao.github.io/convertbeads.github.io/

## 使用

粘贴每行 `色号 颗数` 的库存导出清单，按每包 1000 颗自动转换，点击复制后发给商家。

输入：
```text
A1 1000
A2 2000
A4 2000
```
输出：`A1*1, A2*2, A4*2`

支持空格、Tab、空行、全角字母数字；色号转大写。默认合并重复色号、跳过零数量。不足整包默认提示，可选择向上补齐。格式错误时阻止复制，避免漏单。支持逗号分隔或每行一个。

浏览器若不允许读取剪贴板，可直接使用 Ctrl/Command + V。复制不可用时会选中结果供手动复制。

## 部署与修改

GitHub Settings → Pages → Deploy from a branch → main → / (root)。修改根目录 index.html 即可触发更新。手机和桌面均可使用；也可下载 index.html 直接打开。
