# Theatre Archive

个人观剧数据库，可直接部署到 GitHub Pages。

## 部署

1. 新建 GitHub 仓库。
2. 将本文件夹内所有文件上传到仓库根目录。
3. 打开 Settings → Pages。
4. Source 选择 Deploy from a branch，分支选择 main / root。
5. 等待 GitHub 生成网站地址。

## 数据结构

- 剧目：名称、类型、唯一海报、标签等。
- 演员：演员只建立一次。
- 观剧记录：关联一个剧目和多个演员。

旧版 Theatre Diary 数据会在浏览器中自动迁移为新结构。

## 跨设备同步

在“设置 / 导入导出”中配置 GitHub 用户名、数据仓库、分支、文件路径和 Fine-grained Personal Access Token。建议单独建立一个私有数据仓库，并只给该仓库 Contents 读写权限。

## Excel 导入格式

第一列：时间，例如 `2026.4.12午`。
第二列：剧名。
第三列起：每一列一个演员。

不存在的剧目或演员会自动创建。
