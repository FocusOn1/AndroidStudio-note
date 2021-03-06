# UI设计

----
## <span id="jump目录">目录</span>
1. [UI相关概念](#jump1)  
  1.1.[view](#jump1.1)  
  1.2.[view类常用属性](#jump1.2)  
  1.3.[View Group](#jump1.3)  
  1.4.[Android UI组件的层次结构](#jump1.4)  
2. [控制UI界面](#jump2)  
  2.1[控制UI界面的4种方法](#jump2.1)
3. [布局管理器](#jump3)  
  3.1[什么是布局管理器](#jump3.1)  
  3.2[常用的布局管理器](#jump3.2)  
  3.3[布局管理器嵌套](#jump3.3)
----

# <span id="jump1">一、UI相关概念</span>|[返回目录](#jump目录)

## <span id="jump1.1">1.view</span>|[返回目录](#jump目录)

![image-20210808154000964](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154000964.png)

> ps:
>
> View类位于android.view包中；
>
> View类的子类一般都位于android.widget包中。

## <span id="jump1.2">2.view类常用属性</span>|[返回目录](#jump目录)


| 属性           | 代码格式                                                     |
| -------------- | ------------------------------------------------------------ |
| id属性         | `android:id="@+id/user"`                                                                                                  ![image-20210808154053923](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154053923.png) |
| background属性 | 【图片】`android:background="@mipmap/bg"`                                 ![image-20210808154151067](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154151067.png)                                                                                                      【颜色背景】`android:background="#FF6600"`                                  ![image-20210808154211549](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154211549.png) |
| padding属性    | ![image-20210808154318325](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154318325.png) |

## <span id="jump1.3">3.View Group</span>|[返回目录](#jump目录)

![image-20210808154351668](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154351668.png)

> ViewGroup控制其子组件分布时依赖的内部类
>
> | 类                           |                                                              | 功能                     |
> | ---------------------------- | ------------------------------------------------------------ | ------------------------ |
> | ViewGroup.LayoutParams       | ![image-20210808154442956](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154442956.png) | 控制组件的位置，宽度高度 |
> | ViewGroup.MarginLayoutParams | ![image-20210808154500003](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154500003.png) | 控制子组件的外边距       |

## <span id="jump1.4">4.Android UI组件的层次结构</span>|[返回目录](#jump目录)
![image-20210808154534540](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154534540.png)

# <span id="jump2">二、控制UI界面</span>|[返回目录](#jump目录)

## <span id="jump2.1">1.控制UI界面的4种方法</span>|[返回目录](#jump目录)

| 方法                    |                                                              | 效果                                                         |
| ----------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 使用XML布局文件【推荐】 | ![image-20210808154621929](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154621929.png) | ![image-20210729154725424](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210729154725424.png) |
| 在Java代码中            | ![image-20210729155353308](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154745105.png) | ![image-20210729162957673](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimgimage-20210729162957673.png) |
| 使用XML和Java代码混合   | ![image-20210808154812963](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808154812963.png) | ![image-20210730152400107](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimgimage-20210730152400107.png) |
| 开发自定义的View        | ![image-20210730152325017](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730152325017.png) | <video src="C:/Users/59501/Desktop/%E7%90%AA%E4%BA%9A%E5%A8%9C%E8%AF%B1%E6%8D%95%E5%99%A8.wmv"></video> |



# <span id="jump3">三、布局管理器</span>|[返回目录](#jump目录)

## <span id="jump3.1">1.什么是布局管理器</span>|[返回目录](#jump目录)

![image-20210730161736062](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730161736062.png)

## <span id="jump3.2">2.常用的布局管理器</span>|[返回目录](#jump目录)

| 类型                      | 形态                                                         | 相关组件                                                     |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| RelativeLayout  相对——    | ![image-20210730162454162](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730162454162.png) | ![image-20210730163050798](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730163050798.png) |
| LinearLayout      线性——  | ![image-20210730163839169](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730163839169.png) | ![image-20210730164517802](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730164517802.png)【<LinearLayout>标记】![image-20210730164240081](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730164240081.png) |
| FrameLayout      帧——     | ![image-20210730200301306](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730200301306.png) | ![image-20210730200429425](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730200429425.png) |
| TableLayout        表格—— | ![image-20210731132059859](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210731132059859.png)![image-20210730201304239](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210730201304239.png) |                                                              |
| AbsoluteLayout   网格——   |                                                              |                                                              |
| GridLayout                | ![image-20210731211909517](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210731211909517.png)![image-20210731132025054](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210731132025054.png) | ![image-20210731132549689](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210731132549689.png)![image-20210808160200534](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210808160200534.png) |

## <span id="jump3.3">3.布局管理器嵌套</span>|[返回目录](#jump目录)

![image-20210801163125045](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210801163125045.png)

### 1.布局管理器的嵌套原则

![image-20210801163752875](https://cdn.jsdelivr.net/gh/FocusOn1/myImg/imgimage-20210801163752875.png)

