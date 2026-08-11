# HaizhucodexDesignSkill

一个面向 Codex 与兼容 `SKILL.md` 的 AI 编程代理的前端设计 Skill。它把设计判断、UX 规则、设计系统、可访问组件和最终质量审计组织成一条可执行工作流，帮助代理完成 UI 设计、重构与前端开发。

## 能做什么

- 设计并实现 Landing Page、SaaS、Dashboard、Portfolio、E-commerce 和编辑型网站
- 从模糊需求生成设计简报、视觉方向、页面结构和组件规划
- 为已有项目创建或完善 `DESIGN.md`、颜色、字体、间距、圆角、阴影与动效规则
- 在现有 React、Next.js、Vite、Tailwind 和 shadcn 项目中直接开发
- 审计并改善视觉层级、排版、响应式、无障碍、交互状态与动效性能
- 从 Motion Sites、React Bits、Uiverse、Anime.js 和 Aceternity UI 中选择相关模式与提示词

## 核心编排

该 Skill 会按任务情况调用或模拟以下五类能力：

1. **UI UX Pro Max**：行业 UX 模式、信息架构、颜色、字体和平台约束。
2. **Design MD Collection**：设计语言、Tokens、组件规则和 `DESIGN.md`。
3. **Taste Skill**：视觉判断、构图、差异化和去除常见 AI 风格。
4. **shadcn**：可访问 React 组件基础、表单、对话框、菜单和数据展示。
5. **Impeccable**：最终视觉、UX、响应式和无障碍审计。

## 灵感与模式来源

- **Motion Sites**：滚动叙事、Hero 动效、分段过渡和作品集体验
- **React Bits**：React 动画文本、列表、卡片、背景与交互原语
- **Uiverse**：按钮、输入框、开关、加载器和轻量 Micro-interaction
- **Anime.js**：时间线、SVG、Stagger 和复杂序列动画
- **Aceternity UI**：高级 React Landing Page、Hero、Feature Grid 和背景效果

仓库只保存原创工作流和提示词，不重新分发这些项目的第三方源码。实际引入组件前应核对对应许可证。

## 安装方法

### 方法一：使用 Codex Skill Installer

```text
安装这个 Skill：https://github.com/Liuhaizhu996/HaizhucodexDesignSkill
```

也可以让 Codex 使用 `skill-installer` 从该仓库安装。

### 方法二：Git Clone

```powershell
git clone https://github.com/Liuhaizhu996/HaizhucodexDesignSkill.git "$HOME\.codex\skills\haizhucodex-design-skill"
```

### 方法三：手动复制

将仓库复制到：

```text
%USERPROFILE%\.codex\skills\haizhucodex-design-skill
```

完成后彻底重启 Codex。

## 如何使用

可以显式调用：

```text
使用 $haizhucodex-design-skill，为我的 Next.js SaaS 产品设计并实现一个深色 Landing Page。
```

也可以直接描述任务，Codex 会根据 `description` 自动匹配：

```text
重新设计当前首页。保留现有文案和业务逻辑，改善视觉层级、响应式和动效，并运行构建验证。
```

### 示例一：SaaS Landing Page

```text
使用 $haizhucodex-design-skill，为 AI 数据分析 SaaS 设计首页。目标用户是中小企业运营负责人。使用 shadcn 作为组件基础，参考 Aceternity UI 的高级 Hero 构图和 Motion Sites 的分段过渡，但避免过度动画。直接修改当前项目并运行 lint、typecheck 和 build。
```

### 示例二：Dashboard

```text
使用 $haizhucodex-design-skill，审计并重构当前 Dashboard。重点改善信息密度、导航、表格、筛选器、空状态、键盘操作和移动端布局。不要改变 API 和数据模型。
```

### 示例三：Portfolio

```text
使用 $haizhucodex-design-skill，创建一个有编辑感的设计师 Portfolio。结合 Taste Skill 的排版判断、Motion Sites 的滚动叙事和 React Bits 的文字动画。必须支持 prefers-reduced-motion。
```

### 示例四：已有页面审计

```text
使用 $haizhucodex-design-skill，审计这个前端项目并按影响排序修复 UI 问题。检查视觉层级、字体、间距、颜色对比、Focus、Touch Target、Loading、Empty、Error 和 Disabled 状态。
```

### 示例五：创建设计系统

```text
使用 $haizhucodex-design-skill，根据现有页面提炼一份 DESIGN.md，定义颜色、排版、间距、圆角、阴影、组件、图标和动效规则，然后让现有三个页面统一到该设计系统。
```

## 推荐输入信息

为了获得更稳定的结果，提示词最好包含：

- 产品类型与目标用户
- 用户最重要的任务
- 框架和技术栈
- 品牌关键词或参考页面
- 必须保留的内容与业务行为
- 移动端和无障碍要求
- 希望使用或避免的动画
- 是否允许新增依赖
- 需要运行的验证命令

信息不完整时，Skill 会先检查项目并采用可逆的合理默认值继续工作。

## 工作流程

```text
项目检查
  -> 设计简报
  -> 视觉方向
  -> DESIGN.md / Tokens
  -> 页面与组件规划
  -> shadcn 基础实现
  -> 选择相关动效与高级组件模式
  -> 响应式与无障碍验证
  -> lint / typecheck / test / build
  -> Impeccable 最终审计
```

## 项目结构

```text
HaizhucodexDesignSkill/
├── SKILL.md
├── README.md
├── LICENSE
└── references/
    └── prompt-library.md
```

## 注意事项

- 第三方组件必须检查许可证、框架版本、SSR 和无障碍兼容性。
- 不要为了展示效果叠加多个大型动效。
- 简单 Hover 与状态切换应优先使用 CSS。
- Anime.js 只应用于确实需要 Timeline、Stagger 或 SVG 协调的场景。
- 自定义组件需要补充键盘操作、Focus、Loading、Empty、Error 和 Reduced Motion 状态。

## License

MIT。第三方项目、名称、商标和组件版权归各自所有者。
