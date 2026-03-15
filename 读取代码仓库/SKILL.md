然后这个绿色是增加的，如果有红色就表示删减删减的，然后看他改的差不多就可以点这个保留或者这个取消后，他现在正在做，所以所以现在先不看这个# 读取代码仓库

用于详细读取和分析代码仓库内容的 skill。

## 使用场景

- 用户需要了解项目结构和代码组织
- 用户需要查看特定文件或目录的内容
- 用户需要分析代码仓库的架构和依赖关系

## 操作步骤

### 1. 查看项目结构

```bash
ls -la
tree -L 2
```

### 2. 查看特定文件内容

```bash
cat <文件路径>
cat <目录>/*.<扩展名>
```

### 3. 查看文件统计信息

```bash
find . -type f -name "*.py" | wc -l
find . -type f -name "*.js" | wc -l
```

### 4. 查看关键配置文件

- `package.json` - Node.js 项目配置
- `requirements.txt` - Python 依赖
- `pom.xml` - Java Maven 项目
- `go.mod` - Go 模块
- `Cargo.toml` - Rust 项目

### 5. 查看代码统计

```bash
cloc .
loc --extensions=py,js,ts,java,c,cpp,h --exclude-dir=node_modules
```

## 注意事项

- 优先读取关键配置文件了解项目结构
- 对于大型项目，分目录读取避免信息过载
- 关注 README、文档目录和测试文件
- 注意识别项目使用的语言和框架
