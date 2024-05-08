# flutter：角标-CSDN博客
角标应该非常常见了，以小说app为例，通常会在小说封面的右上角上显示当前未读的章数。

badges
------

**简介**  
[Flutter](https://so.csdn.net/so/search?q=Flutter&spm=1001.2101.3001.7020)的`badges`库是一个用于创建徽章组件的开源库。它提供了简单易用的API，使开发者可以轻松地在Flutter应用程序中添加徽章效果。

**官方文档**  
[https://pub-web.flutter-io.cn/packages/badges](https://pub-web.flutter-io.cn/packages/badges)

**安装**

```
`flutter pub add badges` 

*   1


```

**示例1**

```
`Center(
        child: badges.Badge(
      badgeContent: const Text('3',style: TextStyle(fontSize: 20),),
      child: SizedBox(
        width: 200,
        height: 260,
        child: Image.asset('lib/assets/img/error.jpg',fit: BoxFit.fill,),
      ),
    ));` 

*   1
*   2
*   3
*   4
*   5
*   6
*   7
*   8
*   9


```

![](https://github.com/yogiant333/image/blob/main/image/2024-5-8%2012-40-18/5c4ecb81-7a06-4e1a-b4ca-df75c4853e33.png?raw=true)
  
**示例2**

```
`Center(
        child: badges.Badge(
      position: badges.BadgePosition.topStart(), 
      badgeContent: const Text(
        '3',
        style: TextStyle(fontSize: 20,color: Colors.white),
      ), 
      onTap: () {
        print("点击事件");
      },
      
      badgeStyle: badges.BadgeStyle(
          shape: badges.BadgeShape.square, 
          badgeColor: Colors.blue,
          padding: const EdgeInsets.symmetric(horizontal: 15,vertical: 5),
          borderRadius: BorderRadius.circular(10)),
      child: SizedBox(
        width: 200,
        height: 260,
        child: Image.asset(
          'lib/assets/img/error.jpg',
          fit: BoxFit.fill,
        ),
      ),
    ));` 

*   1
*   2
*   3
*   4
*   5
*   6
*   7
*   8
*   9
*   10
*   11
*   12
*   13
*   14
*   15
*   16
*   17
*   18
*   19
*   20
*   21
*   22
*   23
*   24
*   25


```

**示例3**

```
 `shape: badges.BadgeShape.twitter ,` 

*   1


```

![](https://github.com/yogiant333/image/blob/main/image/2024-5-8%2012-40-18/678b603f-7478-4f37-9c05-1177d414702e.png?raw=true)
  
**示例4**

```
`shape: badges.BadgeShape.instagram ,` 

*   1


```

![](https://github.com/yogiant333/image/blob/main/image/2024-5-8%2012-40-18/0c1e41a2-1aea-4aae-b2a2-7f0f72c2f49f.png?raw=true)

rotated\_corner\_decoration
---------------------------

**简介**  
Flutter中的`rotated_corner_decoration`是一个用于创建旋转圆角装饰的类。它是Flutter框架中的一个内置[装饰器](https://so.csdn.net/so/search?q=%E8%A3%85%E9%A5%B0%E5%99%A8&spm=1001.2101.3001.7020)，可以应用于各种小部件，如容器、按钮、卡片等。

**官方文档**  
[https://pub-web.flutter-io.cn/packages/rotated\_corner\_decoration](https://pub-web.flutter-io.cn/packages/rotated_corner_decoration)

**安装**

```
`flutter pub add rotated_corner_decoration` 

*   1


```

**示例1**

```
`Container(
          width: 200,
          height: 200,
          foregroundDecoration: const RotatedCornerDecoration.withColor(
              color: Colors.red,
              badgeSize: Size(30,30)
          ),
          decoration: BoxDecoration(
            border: Border.all(color: Colors.black,width: 1)
          ),
        )` 

*   1
*   2
*   3
*   4
*   5
*   6
*   7
*   8
*   9
*   10
*   11


```

![](https://github.com/yogiant333/image/blob/main/image/2024-5-8%2012-40-18/945131b9-191a-4800-a8a8-e38fde5326d1.png?raw=true)
  
**示例2**

```
`Container(
      width: 200,
      height: 200,
      foregroundDecoration: const RotatedCornerDecoration.withColor(
          color: Colors.red,
          badgeSize: Size(60, 60), 
          badgePosition: BadgePosition.topStart, 
          spanBaselineShift: 4, 
          textSpan:
              TextSpan(text: 'flutter', style: TextStyle(color: Colors.white))),
      decoration:
          BoxDecoration(border: Border.all(color: Colors.black, width: 1)),
    )` 

*   1
*   2
*   3
*   4
*   5
*   6
*   7
*   8
*   9
*   10
*   11
*   12
*   13


```

![](https://github.com/yogiant333/image/blob/main/image/2024-5-8%2012-40-18/f118ad44-ff39-423d-950e-99e8231cf1f6.png?raw=true)
  
**示例3**

```
`Container(
      width: 200,
      height: 200,
      foregroundDecoration: const RotatedCornerDecoration.withColor(
          color: Colors.red,
          badgeSize: Size(80, 80), 
          badgePosition: BadgePosition.topStart, 
          spanBaselineShift: 4, 
          textSpan:
              TextSpan(text: 'hello\nflutter', style: TextStyle(color: Colors.white))),
      decoration:
          BoxDecoration(border: Border.all(color: Colors.black, width: 1)),
    )` 

*   1
*   2
*   3
*   4
*   5
*   6
*   7
*   8
*   9
*   10
*   11
*   12
*   13


```

![](https://github.com/yogiant333/image/blob/main/image/2024-5-8%2012-40-18/8ea3afdc-321d-4438-b12f-fcb2e94b4fc1.png?raw=true)