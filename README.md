# vim_package
vim插件管理

# 配置

1. 创建目录`~/.vim/pack`
2. 进入目录`cd ~/.vim/pack`
3. 克隆本git：`git clone https://github.com/dachengxi/vim_package.git`
4. 可选步骤：如果`~/.vim/pack/vim_package`目录下没有start或者opt目录，可自行进行创建两个目录
5. 执行`git submodule init`
6. 添加插件，先进入`~/.vim/pack/vim_package`目录下，然后执行：`git submodule add xxxxx start/xxxxx`

# 插件

添加插件先进入`~/.vim/pack/vim_package`目录下

## NERDTree

目录树插件

### 添加插件

`git submodule add https://github.com/preservim/nerdtree.git start/nerdtree`

### 添加文档说明

`vim -u NONE -c "helptags ~/.vim/pack/vim_package/start/nerdtree/doc" -c q`

### 使用

打开目录树：`:NERDTreeToggle`

## vim-easy-align

格式化对齐插件

### 添加插件

`git submodule add https://github.com/junegunn/vim-easy-align.git start/vim-easy-align`

### 添加文档说明

`vim -u NONE -c "helptags ~/.vim/pack/vim_package/start/vim-easy-align/doc" -c q`

### 使用

添加快捷键到`.vimrc`文件中：`xmap ga <Plug>(EasyAlign)`

使用示例：

```bash
1. vim xxx.txt

2. 使用v 进入visual模式

3. 选择需要格式化的内容

4. 使用ga 然后输入格式化条件

```

