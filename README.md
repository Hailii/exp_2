# 实验二
## Android布局
### 线性布局
#### 关键代码
```
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="210dp">
    <LinearLayout android:orientation="horizontal"
        android:layout_width="fill_parent"
        android:layout_height="match_parent"
        android:layout_weight="1">

        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="One,One" />
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="0.8"
            android:text="One,Two"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="One,Three"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="One,Four"/>
    </LinearLayout>
    <LinearLayout android:orientation="horizontal"
        android:layout_width="fill_parent" android:layout_height="fill_parent"
        android:layout_weight="1">
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Two,One"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="0.8"
            android:text="Two,Two"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Two,Three"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Two,Four"/>
    </LinearLayout>
    <LinearLayout android:orientation="horizontal"
        android:layout_width="fill_parent" android:layout_height="fill_parent"
        android:layout_weight="1">
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Three,One"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Three,Two"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Three,Three"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Three,Four"/>
    </LinearLayout>
    <LinearLayout android:orientation="horizontal"
        android:layout_width="fill_parent" android:layout_height="fill_parent"
        android:layout_weight="1">
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Four,One"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="0.8"
            android:text="Four,Two"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Four,Three"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Four,Four"/>
    </LinearLayout>
</LinearLayout>
```
#### 截图
![无法显示](/1.png)
### ConstraintLayout
#### 其中一个控件的代码
```
    <TextView
        android:id="@+id/textView"
        android:layout_width="143dp"
        android:layout_height="98dp"
        android:background="#ffff00"
        android:gravity="center"
        android:text="YELLOW"
        android:textColor="@android:color/background_dark"
        android:textSize="24sp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
```
#### 截图
![无法显示](/2.png)
### 表格布局
#### 关键代码
```
<TableRow>
        <TextView
            android:layout_column="1"
            android:padding="4dp"
            android:text="Open..." />
        <TextView
            android:gravity="right"
            android:padding="4dp"
            android:text="Ctrl-O" />
    </TableRow>
    <TableRow>
        <TextView
            android:layout_column="1"
            android:padding="4dp"
            android:text="Save..." />
        <TextView
            android:gravity="right"
            android:padding="4dp"
            android:text="Ctrl-S" />
    </TableRow>
    <TableRow>
        <TextView
            android:layout_column="1"
            android:padding="4dp"
            android:text="Save As..." />
        <TextView
            android:gravity="right"
            android:padding="4dp"
            android:text="Ctrl-Shift-S" />
    </TableRow>
    <View
        android:layout_height="2dp"
        android:background="#FF909090" />
    <TableRow>
        <TextView
            android:padding="4dp"
            android:text="X" />
        <TextView
            android:padding="4dp"
            android:text="Import..." />
    </TableRow>
    <TableRow>
        <TextView
            android:padding="4dp"
            android:text="X" />
        <TextView
            android:padding="4dp"
            android:text="Export..." />
        <TextView
            android:gravity="right"
            android:padding="4dp"
            android:text="Ctrl-E" />
    </TableRow>
    <View
        android:layout_height="2dp"
        android:background="#FF909090" />
    <TableRow>
        <TextView
            android:layout_column="1"
            android:padding="4dp"
            android:text="Quit" />
    </TableRow>
```
#### 截图
![无法显示](/3.png)
