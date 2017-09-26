# hexo-theme-mip-apollo

Hexo MIP 模板, [在线预览](https://xuexb.github.io/hexo-theme-mip-demo/)，思路来自 [@xuexb/hexo-theme-mip](https://github.com/xuexb/hexo-theme-mip) 和 [@pinggod/hexo-theme-apollo](https://github.com/pinggod/hexo-theme-apollo)

## 安装

```bash
# 安装依赖
npm install --save \
    hexo-browsersync \
    hexo-renderer-jade \
    hexo-generator-feed \
    hexo-generator-sitemap \
    hexo-generator-archive \
    hexo-generator-mip

# 克隆主题
git clone https://github.com/yugasun/hexo-theme-mip-apollo.git themes/mip_apollo
```

> 注意: [hexo-generator-mip](https://github.com/xuexb/hexo-generator-mip) 模块会处理 MIP 规范的标签, 如抽离 `<style>`、处理 `<a>` 标签、处理 `<img>` 标签, 如果不使用 Hexo MIP 相关模板, 请不要安装该模块


## 配置

修改 `_config.yml` 的 `theme` 配置项为 `mip_apollo`:

```yaml
# 启用 mip 主题
theme: mip_apollo
```

## 使用

### 插入图片

由于 [MIP img标签规范](https://www.mipengine.org/examples/mip/mip-img.html) , 在使用图片时必须设置宽高, 如:

```html
<img src="https://dummyimage.com/100x100" width="100" height="100" alt="desc">
```

> 注意:如果你的图片是绝对定位的，请给 `img` 标签添加 `layout="fill"` 属性。


## todo

- [ ] 标签页
- [ ] 搜索页

## contributors

- [@yugasun](https://github.com/yugasun/)
- [@xuexb](https://github.com/xuexb/)

## License

[MIT](./LICENSE)
