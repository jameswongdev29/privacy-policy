# Privacy Policy 托管仓库

本仓库用于托管多个 App 的隐私政策页面，通过 GitHub Pages 对外提供访问。

## 项目结构

```
privacy-policy/
├── CLAUDE.md
├── LICENSE
├── README.md
├── <AppName>/
│   └── index.html      # 该 App 的隐私政策页面
├── <AnotherApp>/
│   └── index.html
└── ...
```

每个 App 对应一个独立的目录，目录名使用 App 名称（PascalCase），目录内放置 `index.html` 作为隐私政策页面。

## 访问路径

部署到 GitHub Pages 后，各 App 的隐私政策访问路径为：

```
https://jameswongdev29.github.io/privacy-policy/<AppName>/
```

例如：`https://jameswongdev29.github.io/privacy-policy/SubLuna/`

## 新增 App 隐私政策

新增隐私政策时，遵循以下规范：

1. 在仓库根目录创建以 App 名称命名的目录（PascalCase）
2. 在该目录下创建 `index.html`
3. HTML 使用英文编写，结构参照 `SubLuna/index.html`
4. 必须包含以下章节：
   - **Effective Date** — 生效日期
   - **Data We Collect** — 数据收集说明
   - **Permissions** — 权限用途说明（根据 App 类型调整标题）
   - **Children** — 儿童隐私声明
   - **Changes** — 政策变更说明
   - **Contact** — 联系方式（邮箱：jameswongdev29@hotmail.com）
5. 如有 iCloud、第三方服务等特殊功能，增加对应章节说明

## 编写原则

- 语言简洁、措辞准确，适用于 App Store 审核
- 如实描述 App 的数据行为，不夸大不遗漏
- 联系邮箱统一使用 `jameswongdev29@hotmail.com`
- 开发者署名统一使用 `Weidi Huang`

## Git 规范

- 主分支：`main`
- 提交信息使用英文，格式：`Add privacy policy for <AppName>` 或 `Update privacy policy for <AppName>`
