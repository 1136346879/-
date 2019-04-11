# -
淘宝城市选择编写

![image](https://github.com/1136346879/flutter-/blob/master/gifStorage/%E5%9F%8E%E5%B8%82%E9%80%89%E6%8B%A9.gif)


代码详细如下：主要逻辑内容在这个类中AreaSelectorDialog.class

布局文件：
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:orientation="vertical"
    android:background="@color/white">
    
    <RelativeLayout
        android:id="@+id/rlTopTip"
        android:layout_width="match_parent"
        android:layout_height="wrap_content">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="配送至"
            android:layout_centerInParent="true"
            android:textSize="@dimen/text_size_16"
            android:textColor="@color/text_color_light"
            android:layout_margin="@dimen/space_10"/>

        <ImageView
            android:id="@+id/ivAreaClose"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:src="@drawable/location_close_dia"
            android:layout_centerVertical="true"
            android:layout_alignParentRight="true"
            android:padding="@dimen/space_10"/>
    </RelativeLayout>
    
    <android.support.design.widget.TabLayout
        android:id="@+id/tab_layout"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="@drawable/background_input_normal"
        app:tabTextColor="@color/text_color_light"
        app:tabSelectedTextColor="@color/text_color_light"
        app:tabMode="scrollable"
        app:tabIndicatorColor="@color/color_orange"
        >
        <android.support.design.widget.TabItem
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="请选择"
            />

    </android.support.design.widget.TabLayout>

    <android.support.v7.widget.RecyclerView
        android:id="@+id/recycler_view"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginLeft="@dimen/space_20"/>
</LinearLayout>

TabLayout是动态添加和减少的
recycleview是动态显示城市列表，由接口控制，及上一级城市code


代码地址：https://github.com/1136346879/picture_dx

