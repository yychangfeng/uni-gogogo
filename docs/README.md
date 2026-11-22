# wit-go 网页版（iPhone / 桌面浏览器）

安卓版 wit-go 的「只读版」。浏览器拿不到教务系统登录后的页面（跨域），所以这里不做自动导入，
改成：**安卓端导出课表文件 → 这里选文件导入**，数据只存在这台设备的浏览器本地。

## 文件

- `index.html`：整个应用（课表渲染、周切换、课程详情、导入文件），单文件、无外部依赖
- `manifest.webmanifest`：添加到主屏幕用的应用信息
- `sw.js`：离线缓存（装到主屏幕后没网也能看）
- `icon-192.png` / `icon-512.png` / `apple-touch-icon.png`：图标

## 部署（GitHub Pages）

1. 把这个 `docs/` 目录提交到仓库 `main` 分支根目录
2. 仓库 Settings → Pages → Source 选「Deploy from a branch」→ Branch 选 `main`、目录选 `/docs` → Save
3. 等 1 分钟左右：`https://yychangfeng.github.io/wit-go/`

## iPhone 上装

1. Safari 打开上面的网址（必须 Safari，微信内打开不行）
2. 底部「分享」→「添加到主屏幕」
3. 之后从桌面图标打开，就是全屏、没地址栏的样子；没网也能看

## 限制（和安卓版的差别）

- 不能自动导入教务系统课表，只能导入安卓版导出的 `.json`
- 没有上课提醒（iOS 的网页无法定时弹本地通知）
- 没有小组件、没有成绩查询
- 浏览器清缓存 / 长期不用，本地数据可能被系统回收——重要课表请留一份 `.json` 备份