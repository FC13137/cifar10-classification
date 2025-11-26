# 如何上传项目到 GitHub

## 方法一：使用 Git 命令行（推荐）

### 步骤 1: 初始化 Git 仓库
在项目文件夹中打开 PowerShell 或命令提示符，运行：
```bash
git init
```

### 步骤 2: 添加所有文件
```bash
git add .
```

### 步骤 3: 提交文件
```bash
git commit -m "Initial commit: CIFAR-10 classification project"
```

### 步骤 4: 在 GitHub 上创建新仓库
1. 登录 GitHub (https://github.com)
2. 点击右上角的 "+" 号，选择 "New repository"
3. 填写仓库名称（例如：`cifar10-classification`）
4. 选择 Public 或 Private
5. **不要**勾选 "Initialize this repository with a README"（因为我们已经有了）
6. 点击 "Create repository"

### 步骤 5: 连接本地仓库到 GitHub
GitHub 会显示一个页面，复制其中的命令。通常是：
```bash
git remote add origin https://github.com/你的用户名/仓库名.git
git branch -M main
git push -u origin main
```

### 步骤 6: 推送代码
运行上面的命令，或者手动运行：
```bash
git remote add origin https://github.com/你的用户名/仓库名.git
git branch -M main
git push -u origin main
```

如果提示输入用户名和密码，使用 GitHub 的 Personal Access Token（不是密码）。

---

## 方法二：使用 GitHub Desktop（图形界面，更简单）

### 步骤 1: 下载 GitHub Desktop
从 https://desktop.github.com/ 下载并安装

### 步骤 2: 登录 GitHub 账号

### 步骤 3: 添加本地仓库
1. 打开 GitHub Desktop
2. 点击 "File" → "Add Local Repository"
3. 选择你的项目文件夹
4. 如果提示需要初始化，点击 "create a repository"

### 步骤 4: 提交并推送
1. 在 GitHub Desktop 中，你会看到所有更改的文件
2. 在左下角填写提交信息（例如："Initial commit"）
3. 点击 "Commit to main"
4. 点击 "Publish repository" 按钮
5. 输入仓库名称，选择 Public/Private
6. 点击 "Publish Repository"

---

## 方法三：直接在 GitHub 网页上传（最简单，但只适合小项目）

1. 在 GitHub 创建新仓库（步骤同方法一的步骤 4）
2. 创建后，点击 "uploading an existing file"
3. 拖拽你的三个 .ipynb 文件、README.md 和 .gitignore 到页面上
4. 填写提交信息，点击 "Commit changes"

---

## 注意事项

- ✅ 三个 .ipynb 文件会被上传
- ✅ README.md 会被上传（项目说明）
- ✅ .gitignore 会被上传（忽略不需要的文件）
- ❌ 模型文件（.pt, .pth）不会被上传（已在 .gitignore 中）
- ❌ 数据文件夹不会被上传（已在 .gitignore 中）

## 如果遇到问题

**问题：提示需要认证**
- 解决方案：使用 Personal Access Token 而不是密码
- 生成 Token：GitHub → Settings → Developer settings → Personal access tokens → Generate new token

**问题：文件太大**
- Jupyter notebook 文件通常不会太大，但如果遇到问题，可以压缩后再上传

