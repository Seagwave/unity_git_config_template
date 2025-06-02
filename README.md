## 使用方法

### Windows
在unity项目根目录打开powershell然后复制下方代码执行
```powershell
@(".gitattributes", ".gitignore") | ForEach-Object {
    Invoke-WebRequest -Uri "https://raw.githubusercontent.com/Seagwave/unity_git_config_template/master/$_" -OutFile $_
}
```

### Git关闭autocrlf
```powershell
# 为当前仓库设置
git config core.autocrlf false

# 或者，为全局设置（影响所有仓库）
git config --global core.autocrlf false
```
