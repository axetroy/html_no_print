收集几种方案，用于防止页面被打印出来。

1. 模糊法

页面失去焦点时，模糊页面，使其打印的页面也模糊。

有效：Chrome/Firefox
无效：IE （模糊无法使用，但可以在 IE 环境使其完全空白作为备选方案）

这个方案体验稍差

[Demo](https://axetroy.github.io/html_no_print/blur_mask.html)

2. css media 方法

浏览器可以自定义打印模式下的 CSS 样式，在打印模式下，隐藏页面所有内容，从而阻止打印

有效：Chrome/Firefox/IE

这个方案对于用户来说，无感知

[Demo](https://axetroy.github.io/html_no_print/css_media.html)

3. 阻止浏览器默认的打印快捷键

默认的浏览器快捷键是 CTRL+P，可以通过阻止快捷键打印

这个方案只能阻止页面内的快捷键，仍然可以通过其他途径触发打印

[Demo](https://axetroy.github.io/html_no_print/block_shotcut.html)

4. 覆盖 javascript 的 print 方法

Javascript 内置了 print 方法，可以覆盖 print 方法，防止其他的 javascript 代码调用打印

这个方案只能阻止 javascript 层面的打印 ，仍然可以通过其他途径触发打印

[Demo](https://axetroy.github.io/html_no_print/overrite_javascript_print.html)

结合以上几个方法，基本上阻止大部分的打印
