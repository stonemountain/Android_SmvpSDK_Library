Android_SmvpSDK_Library
=======================
重要更新说明：Demo不再提供Token，有需要请联系石山视频技术支持,QQ: 2878649713。

使用AndroidStudio开发时，只需要在原工程添加For_AndroidStudio/SmvpSDK.aar，导入方法如下：
1.点击File--->New Module，选择“Import .JAR or .AAR Package”---->Next,选择SmvpSDK.aar包，填写“Subproject name”，例如“SmvpSDK”，点击“finish”。
2.点击File--->Project Structure,选择左侧的Project，然后选择页面中间位置的“Dependencies”，点击最右侧的“+”，选择“3.Module Dependency”，选择“SmvpSDK”。点击“OK”。
3.点击“Build--->Clean Project”
4.然后用同样的方法导入ijkmediaplayer

使用Eclipse开发时，只需要使用For_Eclipse目录下的文件,SmvpSDK是Android Library Project，把SmvpSDK添加到原工程即可。具体如下：
1.导入SmvpSDK到Eclipse，
2.在Package Explorer中, 鼠标右键项目文件夹，点击 Properties.
3.在Properties 窗口, 选择"Android" ，Library属性显示在右下边.
4.点击Add ，打开了Project Selection对话框.
5.从可用库项目列表选择一个项目，然后点击 OK.
6.对话框关闭之后点击 Apply （在Properties窗口）,点击 OK 关闭Properties 窗口.
7.修改APP的AndroidManifest.xml,添加以下内容:
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.RECEIVE_USER_PRESENT" />

        <activity
            android:name="cn.smvp.android.sdk.view.PlayVideoActivity"
            android:configChanges="keyboardHidden|orientation|screenSize"
            android:screenOrientation="landscape" />
        <activity
            android:name="cn.smvp.android.sdk.impl.WebViewActivity"
            android:label="@string/title_activity_web_view"
            android:theme="@android:style/Theme.Holo.Light"
            android:windowSoftInputMode="adjustPan|stateHidden" />
7.点击Project--->Clean

