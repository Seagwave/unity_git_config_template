## 使用方法

### Windows
复制进powershell中执行
```powershell
@(".gitattributes", ".gitignore") | ForEach-Object {
    Invoke-WebRequest -Uri "https://raw.githubusercontent.com/Seagwave/unity_git_config_template/master/$_" -OutFile $_
}
```

