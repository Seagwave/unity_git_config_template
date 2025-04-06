## 使用方法

### Windows
在unity项目根目录打开powershell然后复制下方代码执行
```powershell
@(".gitattributes", ".gitignore") | ForEach-Object {
    Invoke-WebRequest -Uri "https://raw.githubusercontent.com/Seagwave/unity_git_config_template/master/$_" -OutFile $_
}
```

