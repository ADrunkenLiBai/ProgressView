# ProgressView
material design currentProgress view（material design 风格进度条样式）

# Usage Example

in the build.gradle:
```
compile 'com.whathappen:progresslibrary:1.0.2'
```

<li>write 'com.whathappen.progresslibrary.view.CircleProgress' in you layout.xml file:

```xml
	<com.whathappen.progresslibrary.view.CircleProgress
        android:id="@+id/circle_progress"
        android:layout_width="match_parent"
        android:layout_height="200dp"
        android:padding="10dp"
        cp:backgroundColor="@android:color/white"
        cp:dialTextSize="8sp"
        cp:currentProgress="32"
        cp:progressType="gradientType_Dial"
        cp:progressValueStyle="outerValueTypeShowDial"/>
```

<li>write 'com.whathappen.progresslibrary.view.ImageProgress' in you layout.xml file:

```xml
    <com.whathappen.progresslibrary.view.ImageProgress
        android:id="@+id/image_progress"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center_horizontal"
        android:padding="10dp"
        ip:currentProgress="25"
        ip:backgroundIcon="@mipmap/tabbar_compose_friends_neo" />
```

<li>write 'com.whathappen.progresslibrary.view.LinearProgress' in you layout.xml file:

```xml
    <com.whathappen.progresslibrary.view.LinearProgress
        android:id="@+id/linear_progress"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_gravity="center_horizontal"
        android:layout_marginTop="20dp"
        android:padding="10dp"
        lp:currentProgress="32" />
```

# Effect
><li>CircleProgress Effect:

![effect](https://github.com/whatshappen/ProgressView/blob/master/screen_shot/dialogStyle.gif)<br>
><li>ImageProgress Effect:

![effect](https://github.com/whatshappen/ProgressView/blob/master/screen_shot/imageProgress.gif)<br>
><li>LinearProgress Effect:
![effect](https://github.com/whatshappen/ProgressView/blob/master/screen_shot/linearProgress.gif)<br>

# Special Note
<p style='color:red'>When setting currentProgress view the properties in the code, be sure to builder().</p>

# Readme
#### CircleProgress attrs:
> * strokeWidth: Progress bar width (进度条宽度)
> * maxProgress: Biggest currentProgress (最大进度)
> * currentProgress: Current currentProgress (当前进度)
> * startAngle: Starting angle (开始角度)
> * backgroundColor: Background color (进度条默认颜色)
> * progressColor: Progress color (进度颜色)
> * textColor: Progress value font color (进度值字体颜色)
> * textSize: Progress value font size(进度值字体大小)
> * progressColors_start: Gradation start color (渐变色样式开始颜色)
> * progressColors_center: Gradation center color (渐变色样式中间颜色)
> * progressColors_end: Gradation end color (渐变色样式结束颜色)
> * progressType: Progress style (进度值样式：默认，渐变，刻度)
> * dialDefaultColor: Dial color (刻度颜色)
> * singleDialWidth: Dial width (刻度宽度)
> * lineWidth: Dial interval width (刻度间隔宽度)
> * progressValueStyle: Progress value style (进度值显示风格)
> * progressValueType: Progress value type (进度值风格:float,int)
> * dialTextSize: Dial font size (刻度值字体大小)

#### ImageProgress attrs:
> * strokeWidth: Progress bar width (进度条宽度)
> * maxProgress: Biggest currentProgress (最大进度)
> * currentProgress: Current currentProgress (当前进度)
> * backgroundColor: Background color (进度条默认颜色)
> * progressColor: Progress color (进度颜色)
> * textColor: Progress value font color (进度值字体颜色)
> * textSize: Progress value font size(进度值字体大小)
> * progressColors_start: Gradation start color (渐变色样式开始颜色)
> * progressColors_center: Gradation center color (渐变色样式中间颜色)
> * progressColors_end: Gradation end color (渐变色样式结束颜色)
> * progressShaderType: Gradient style (渐变样式)
> * hasTextHint: Whether there is a currentProgress value prompt (是否有进度值提示)
> * backgroundIcon: Background icon (背景图片)
> * progressIndexAndOri: Progress value direction and position (进度值起点和方向)
> * progressStyle: currentProgress style (进度样式)
> * hasLastText: Whether to display currentProgress value when loaded to 100% (加载到100%是否还显示进度值)
> * hasLoadingBackground: Is there a background to load (是否有加载背景)
> * progressLoadingBackground: Progress loading background (加载进度时,图片上层背景颜色)
> * roundRect: Corner radius (圆角半径)

#### LinearProgress attrs:
> * maxProgress: Biggest currentProgress (最大进度)
> * currentProgress: Current currentProgress (当前进度)
> * backgroundColor: Background color (进度条默认颜色)
> * progressColor: Progress color (进度颜色)
> * textColor: Progress value font color (进度值字体颜色)
> * textSize: Progress value font size(进度值字体大小)
> * progressColors_start: Gradation start color (渐变色样式开始颜色)
> * progressColors_center: Gradation center color (渐变色样式中间颜色)
> * progressColors_end: Gradation end color (渐变色样式结束颜色)
> * progressStyle: currentProgress style (进度样式)
> * percentPadding: Progress value padding (进度值padding)
> * roundRectX: Fillet X-axis radius (圆角X轴半径)
> * roundRectY: Fillet Y-axis radius (圆角Y轴半径)

# License
Copyright 2018 whatshappen

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
