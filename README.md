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



```

 BannerView(
          indicatorBg: ColorUtils.c_ffffff,
          indicatorColor: ColorUtils.c_63ca6c,
          indicatorSelectColor: ColorUtils.c_ff0000,
          indicatorAlignmentPos: MainAxisAlignment.end,
          indicatorSize:SizeUtils.px_5,
          onBannerClickListener: (index, itemData) {
            print('liuze${itemData.title}');
          },
          data: data2,
          buildTitle: (int index, itemData) {
            return  Text(itemData.title);
          },
          buildItem: (int index, itemData) {
            return Container(
              child: Image.network(
                itemData.url,
                fit: BoxFit.fill,
              ),
            );
          },
        ),

```
