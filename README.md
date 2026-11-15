# 豆瓣小组资料管理台

一个适配电脑和手机浏览器的静态网页管理工具，适合通过 GitHub Pages 发布。

## 当前版本包含
- 响应式桌面端与移动端界面
- 本地账号档案管理
- 小组资料手动录入、编辑、删除和筛选
- 本地历史记录（localStorage）
- JSON 备份与导入
- 仅导出“已人工核验”记录的 Excel
- 不需要自建服务器

## 重要说明
当前版本是本地资料管理工具，不会自动访问豆瓣或批量查询他人的成员关系。仅整理本人或已获得明确授权的数据；不绕过登录、隐私设置或访问限制。

数据保存在每位访问者自己的浏览器中。GitHub Pages 不会同步访问者的 localStorage。更换浏览器/设备或清除站点数据可能导致记录丢失，请定期导出 JSON 备份。

## 本地预览
直接用浏览器打开 `index.html` 即可。Excel 导出功能首次使用时需要联网加载 SheetJS。

## 发布到 GitHub Pages
1. 在 GitHub 新建一个公开仓库，例如 `douban-group-manager`。
2. 上传 `index.html` 和 `README.md` 到仓库根目录。
3. 进入仓库 `Settings` → `Pages`。
4. 在 `Build and deployment` 中选择 `Deploy from a branch`。
5. Branch 选择 `main`，目录选择 `/(root)`，点击 `Save`。
6. 等待 GitHub Pages 构建完成，页面会显示公开网址，通常形如 `https://你的用户名.github.io/douban-group-manager/`。

## 数据备份
在页面顶部点击“备份数据”，会下载 JSON 文件。换设备后进入“本地历史”→“导入备份”恢复。
