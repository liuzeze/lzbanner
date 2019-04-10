# lzbanner

A new Flutter package.

## Getting Started

This project is a starting point for a Dart
[package](https://flutter.io/developing-packages/),
a library module containing code that can be shared easily across
multiple Flutter or Dart projects.

For help getting started with Flutter, view our 
[online documentation](https://flutter.io/docs), which offers tutorials, 
samples, guidance on mobile development, and a full API reference.

<table align="center">
    <tr align="center">
      <td><img src="https://github.com/liuzeze/lzbanner/blob/master/screenshort/1.jpg" width="280" height="480"/></td>
        <td><img src="https://github.com/liuzeze/lzbanner/blob/master/screenshort/2.jpg" width="280" height="480"/></td>
         <td><img src="https://github.com/liuzeze/lzbanner/blob/master/screenshort/3.jpg" width="280" height="480"/></td>
    </tr>
        
</table>


### 使用方式  demo  https://github.com/liuzeze/Flutter_Demo/blob/master/lib/ui/page/news.dart
```

 BannerView(
          indicatorBg: ColorUtils.c_ffffff,//指示器背景颜色
          indicatorColor: ColorUtils.c_63ca6c, //指示器未选中颜色
          indicatorSelectColor: ColorUtils.c_ff0000,//指示器选中颜色
          indicatorAlignmentPos: MainAxisAlignment.end,//指示器位置 底部的左中 右 三个位置
          indicatorSize:SizeUtils.px_5,//小圆点半径
          onBannerClickListener: (index, itemData) {
            //点击事件
            print('liuze${itemData.title}');
          },
          data: data2,//数据源
          buildTitle: (int index, itemData) {
          //标题控件
            return  Text(itemData.title);
          },
          buildItem: (int index, itemData) {
          //背景图片
            return Container(
              child: Image.network(
                itemData.url,
                fit: BoxFit.fill,
              ),
            );
          },
        ),

```
