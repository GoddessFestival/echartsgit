


自定义构建pie饼图：
echarts 已经提供了构建脚本 echarts/build/build.js


查看构建脚本的使用方法
node node_modules/echarts/build/build.js --help  
-i 代码入口文件
-o 生成的bundle文件
--min 压缩文件（默认不压缩），并且去多余的打印错误信息的代码，形成生产环境可用的文件。
--lang <language shortcut or file path>：语言默认是中文。--lang en使用英文
--sourcemap:输出source.map,便于调试
--format：输出格式，可选'umb'（默认）、'amd'、'iife'、'cjs'、'es'

定义入口文件
myProject/echarts.custom.js（引用所需的echarts模块）
// 引入 echarts 主模块。
export * from 'echarts/src/echarts';
// 引入饼图。
import 'echarts/src/chart/pie';
// 在这个场景下，可以引用 `echarts/src` 或者 `echarts/lib` 下的文件（但是不可混用），


使用命令行构建
node node_modules/echarts/build/build.js --min -i echarts.custom.js -o lib/echarts.custom.min.js























怎样在README.md中添加图片：
1、在github上的仓库建立一个存放图片的文件夹，文件夹名字随意。如：img-folder
2、将需要在READNE.md中显示的图片，push到img-folder文件夹中。
3、然后打开github官网，进入仓库的img-folder文件夹中，找到图片的地址
4、在README.md中填入：

![Image text](https://raw.githubusercontent.com/hongmaju/light7Local/master/img/productShow/20170518152848.png)

注：![Image text]这个标识不可缺少，不然就显示文字了。

Image text：指的是如果图片不存在了，要显示的文字说明。
