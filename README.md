# MultiLineRadioGroup
解决多行显示radiobutton,radiobutton不互斥的问题
#### 使用步骤
##### 1添加 jitpack

``` 
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  ```
  ##### 2添加依赖
  ```
  	        compile 'com.github.meijingkang:multilineradiogroup:v0.0.1'
  ```
  ##### 3布局文件中使用
   ```
   <org.mj.multilinecheckgroup.views.MultiLineRadioGroup
 android:layout_width="match_parent"
 android:id="@+id/radioGroup"
 android:layout_height="wrap_content"
 android:orientation="vertical">

 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:orientation="horizontal">

 <RadioButton
 style="@style/recharge_btn_money_style"
 android:id="@+id/rb_30"
 android:text="30元" />

 <RadioButton
 style="@style/recharge_btn_money_style"
 android:id="@+id/rb_50"
 android:text="50元" />

 <RadioButton
 style="@style/recharge_btn_money_style"
 android:id="@+id/rb_100"
 android:text="100元" />

 </LinearLayout>
 <LinearLayout
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:orientation="horizontal">

 <RadioButton
 style="@style/recharge_btn_money_style"
 android:id="@+id/rb_200"
 android:text="200元" />

 <RadioButton
 style="@style/recharge_btn_money_style"
 android:id="@+id/rb_300"
 android:text="300元" />

 <RadioButton
 style="@style/recharge_btn_money_style"
 android:id="@+id/rb_500"
 android:text="500元" />

 </LinearLayout>
 </org.mj.multilinecheckgroup.views.MultiLineRadioGroup>
   ```
   
   #### 代码中监听选中的id和原生的RadioGroup一样
