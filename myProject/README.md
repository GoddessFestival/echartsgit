


�Զ��幹��pie��ͼ��
echarts �Ѿ��ṩ�˹����ű� echarts/build/build.js


�鿴�����ű���ʹ�÷���
node node_modules/echarts/build/build.js --help  
-i ��������ļ�
-o ���ɵ�bundle�ļ�
--min ѹ���ļ���Ĭ�ϲ�ѹ����������ȥ����Ĵ�ӡ������Ϣ�Ĵ��룬�γ������������õ��ļ���
--lang <language shortcut or file path>������Ĭ�������ġ�--lang enʹ��Ӣ��
--sourcemap:���source.map,���ڵ���
--format�������ʽ����ѡ'umb'��Ĭ�ϣ���'amd'��'iife'��'cjs'��'es'

��������ļ�
myProject/echarts.custom.js�����������echartsģ�飩
// ���� echarts ��ģ�顣
export * from 'echarts/src/echarts';
// �����ͼ��
import 'echarts/src/chart/pie';
// ����������£��������� `echarts/src` ���� `echarts/lib` �µ��ļ������ǲ��ɻ��ã���


ʹ�������й���
node node_modules/echarts/build/build.js --min -i echarts.custom.js -o lib/echarts.custom.min.js























������README.md�����ͼƬ��
1����github�ϵĲֿ⽨��һ�����ͼƬ���ļ��У��ļ����������⡣�磺img-folder
2������Ҫ��READNE.md����ʾ��ͼƬ��push��img-folder�ļ����С�
3��Ȼ���github����������ֿ��img-folder�ļ����У��ҵ�ͼƬ�ĵ�ַ
4����README.md�����룺

![Image text](https://raw.githubusercontent.com/hongmaju/light7Local/master/img/productShow/20170518152848.png)

ע��![Image text]�����ʶ����ȱ�٣���Ȼ����ʾ�����ˡ�

Image text��ָ�������ͼƬ�������ˣ�Ҫ��ʾ������˵����
