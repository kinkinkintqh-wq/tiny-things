# Tiny Things｜小东西制造所

可爱的小东西，也能有可以检查的规则。把按钮、骰子、信封与音乐拼成可以送给朋友的小礼物，接收者打开链接即可试玩，无需钱包。

![Tiny Things](tiny-things-logo-256.png)

## 源码与复现

[下载完整源码（201 个文件）](tiny-things-source-20261112.zip)。当前浏览器登录账号与 GitHub 插件账号不同，先以完整源码包交付；包内保留正确目录结构、README、锁文件、测试和验证素材。解压后从项目根目录运行：

```sh
npm --prefix apps/web ci
npm --prefix packages/tapeout-adapter ci --ignore-scripts
npm test
npm run dev
```

打开 http://127.0.0.1:3846 。无需数据库即可制作、预览、导入导出和快照试玩。Node.js 22+，本地验证24.18.0。

压缩包 SHA256：`50529b78ebe1b98963078000157836f470c393a534bb2aff9a5c1cbe632f8b13`。包内 SOURCE-SHA256.json 记录逐文件指纹。

## TapeOut × X Layer

- 主网 chain ID 196；共享处理器 #414：`0x9e2849c04A513FE64db07521cBE52d078d905c0E`。
- 候选规则：累计12点（390 NAND＋8 LATCH）、收集三个6（397 NAND＋8 LATCH）。
- 正式流片、真实电路ID、正式运行绑定及公网网址仍待确认。这里不使用模拟ID或虚构交易。
- 规则核对失败时保留原状态；只读运行不要求试玩者签名。已完成53项/12文件测试及生产构建，合成测试不等于正式链上验收。

## 参赛材料

[项目介绍与商业计划草稿](project-description.md) · [Demo脚本](demo-script.md) · [源码指纹](SOURCE-PACKAGE.json)

基础试玩计划免费，未来探索主题皮肤与创作者模板包，尚未实现收费。分享快照包含明文，不是加密私信；随机数与进度由浏览器提供。红包、资金托管和分账未实现。三首配乐为项目原创合成循环，字体许可随源码提供，项目未额外授予整体开源许可。

正式流片和公网验证完成后，再补齐最终链接与演示视频。
