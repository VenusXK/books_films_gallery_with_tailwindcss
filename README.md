# 我看过的书籍和电影陈列馆
# My Books and Film Gallery

一个基于 `tailwindcss` 的纯前端项目，记录了我看过的书籍📕和电影🎞️

A pure front-end project based on tailwindcss which records the books📕 and movies🎞️ I've seen

项目链接：http://www.venusxk.com/media.html

Project link: http://www.venusxk.com/media.html

## 界面效果 `Interface Effects`

<br>
<div align=center>
    <img decoding="async" src="./readme_pic/gallery.jpg" width="80%" >
<br>    
图1 界面效果

Figure 1 Interface effects
</div>

## 编辑 `css` `Edit the CSS`

### 1. 安装 `tailwindcss` `Install tailwindcss` 
```nodejs
npm install -D tailwindcss
npx tailwindcss init
```
### 2. 在 `tailwind.config.js` 下设置使用到 `tailwindcss` 的文件的目录 `Configure your template paths`
```json
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### 3. 在 `input.css` 下输入基本配置 `Add the Tailwind directives to your CSS`
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### 4. 启动 `tailwindcss` `CLI` 构建过程 `Start the Tailwind CLI build process`
>**说明：** 目录下 `input_media.css` 文件为输入的 `css` 文件，`output_media.css` 文件为输出的 `css` 文件，根据 `tailwindcss` 框架的要求，在cmd下执行 `npx tailwindcss -i input_media.css -o output_media.css` 语句实现 `css` 文件的输出，输出的 `css` 文件为使用到的 `tailwindcss` 全部文件，在 `html` 中通过 `link` 包含 `output_media.css`。

```cmd
npx tailwindcss -i input_media.css -o output_media.css
```

> 修改 `input_media.css` 文件下的属性，即可改变样式