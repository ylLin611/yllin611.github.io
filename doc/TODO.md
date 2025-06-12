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

## 添加tailwindcss
