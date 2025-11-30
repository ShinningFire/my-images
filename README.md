# my-images

一个用于在线存储图片的 GitHub 仓库。将本地图片上传到此仓库后，可以通过 URL 直接在浏览器中访问。

## 📁 目录结构

```
my-images/
├── images/          # 存放所有上传的图片
│   └── .gitkeep     # 占位文件，保持目录结构
└── README.md        # 使用说明
```

## 🚀 使用方法

### 1. 上传图片

#### 方法一：通过 GitHub 网页上传

1. 进入 [images 目录](./images)
2. 点击 "Add file" → "Upload files"
3. 拖拽或选择要上传的图片
4. 填写 commit 信息，点击 "Commit changes"

#### 方法二：通过 Git 命令行上传

```bash
# 克隆仓库
git clone https://github.com/ShinningFire/my-images.git
cd my-images

# 将图片复制到 images 目录
cp /path/to/your/image.png images/

# 提交并推送
git add images/
git commit -m "Add new image"
git push origin main
```

### 2. 获取图片访问链接

上传图片后，可以通过以下 URL 格式在浏览器中访问：

```
https://raw.githubusercontent.com/ShinningFire/my-images/main/images/<your-image-filename>
```

**示例：**
- 如果上传了 `example.png`，访问链接为：
  ```
  https://raw.githubusercontent.com/ShinningFire/my-images/main/images/example.png
  ```

### 3. 在 Markdown 中使用

```markdown
![图片描述](https://raw.githubusercontent.com/ShinningFire/my-images/main/images/<your-image-filename>)
```

### 4. 在 HTML 中使用

```html
<img src="https://raw.githubusercontent.com/ShinningFire/my-images/main/images/<your-image-filename>" alt="图片描述">
```

## 📝 注意事项

- 建议使用有意义的文件名，便于管理
- 支持常见图片格式：PNG、JPG、JPEG、GIF、SVG、WebP 等
- 文件名避免使用中文和特殊字符，推荐使用英文和数字
- GitHub 单个文件大小限制为 100MB

## 📌 快速链接生成

将图片上传到 `images` 目录后，只需将下面模板中的 `文件名` 替换为你的图片文件名：

```
https://raw.githubusercontent.com/ShinningFire/my-images/main/images/<filename>
```