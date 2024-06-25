要在Git上新建一个仓库并提交本地代码，你可以按照以下步骤进行操作：

### 1. 在GitHub上创建新仓库

1. **登录GitHub**：确保你已经登录到你的GitHub账号。
   
2. **创建新仓库**：
   - 点击右上角的加号图标，选择"New repository"。
   - 给仓库起一个名称，填写描述（可选），选择公开或私有。
   - 不要勾选"Initialize this repository with a README"，因为我们要将本地代码推送到仓库。

3. **创建仓库**：
   - 点击"Create repository"按钮，新仓库就创建好了。

### 2. 在本地设置Git并提交代码

接下来，你需要在本地设置Git，并提交你的代码到新创建的仓库。

1. **在Ubuntu终端设置Git**：

   打开终端，执行以下命令来配置你的Git信息（如果你还没有配置过）：
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```

2. **克隆新仓库到本地**：

   在终端中，进入你希望存放项目的目录，并执行以下命令来克隆刚刚创建的仓库到本地：
   ```bash
   git clone https://github.com/your-username/new-repo.git
   ```
   替换 `https://github.com/your-username/new-repo.git` 中的 `your-username` 为你的GitHub用户名，`new-repo` 为你刚刚创建的仓库名称。

3. **添加和提交本地代码**：

   - 将你的代码复制到克隆下来的目录中。
   - 在终端进入新建的仓库目录：
     ```bash
     cd new-repo
     ```
   - 添加你的所有文件到Git仓库：
     ```bash
     git add .
     ```
   - 提交你的代码并添加提交信息：
     ```bash
     git commit -m "Initial commit"
     ```

4. **推送到GitHub**：

   - 将本地的提交推送到GitHub：
     ```bash
     git push origin master
     ```
     如果你使用的是主分支名称不是 `master`，请将命令中的 `master` 替换为你的分支名称。

现在，你的本地代码已经提交到了GitHub上的新仓库中。可以在GitHub页面上刷新，查看是否成功推送了代码。