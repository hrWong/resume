# 使用说明

## 快速开始

1. **克隆仓库**
   ```bash
   git clone https://github.com/你的用户名/resume.git
   cd resume
   ```

2. **编辑个人信息**
   - 修改 `texs/header_with_photo.tex` 中的姓名、联系方式等
   - 替换 `images/avatar.jpg` 为你的头像
   - 编辑 `texs/sections.tex` 中的简历内容

3. **编译简历**
   ```bash
   make
   # 或者
   xelatex resume-zh_CN.tex
   ```

## 自定义选项

### 切换标题样式
在 `resume-zh_CN.tex` 中修改：
```latex
\settitlelinestyle{default}    % 默认样式
\settitlelinestyle{partialbg}  % 部分背景色
\settitlelinestyle{fullbg}     % 全背景色
```

### 修改颜色
在 `resume.cls` 中修改颜色定义：
```latex
\definecolor{cyanbg}{HTML}{f0fafa}
\definecolor{cyanfg}{HTML}{00a6a7}
```

## 示例文件

参考 `texs/sections_example.tex` 了解如何使用各种命令。

## 环境要求

- LaTeX发行版（推荐TeX Live 2023+）
- XeLaTeX编译器
- 中文字体支持 