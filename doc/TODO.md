## prettier格式化

```
pnpm i -D prettier prettier-plugin-tailwindcss prettier-plugin-astro
```

新建 .prettierrc.json

```json
{
  "plugins": ["prettier-plugin-tailwindcss", "prettier-plugin-astro"],
  "overrides": [
    {
      "files": "*.astro",
      "options": {
        "parser": "astro"
      }
    }
  ]
}
```

执行：

```bash
pnpm exec prettier . --write
```

## 添加tailwindcss V4

```bash
pnpm astro add tailwind
```

global.css 中添加

```css
@import "tailwindcss";
```

## 基础文件替换

### 标题

更改 consts.ts

### logo

在[favicon生成网站](https://realfavicongenerator.net/)生成文件，复制到`public`文件夹下

修改 `BaseHead.astro` 组件

```html
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png" />
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png" />
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png" />
<link rel="manifest" href="/site.webmanifest" />
```

### footer
