# FirefoxCustomizations
本人定制火狐使用的CSS等，适用于Windows系统

### 使用前建议
打开火狐浏览器，在地址栏输入`about:config`，搜索并设置以下首选项：
<p>
<code>browser.tabs.allow_transparent_browser</code><br>
<code>browser.theme.native-theme</code><br>
<code>widget.non-native-theme.use-theme-accent</code><br>
<code>widget.windows.mica</code><br>
将以上首选项设为<code>true</code><br><br>
<code>widget.windows.mica.popups</code>设为<code>2</code><br>
<code>widget.windows.mica.toplevel-backdrop</code>设为<code>1</code><br>
</p>

**不建议使用非默认“系统主题—自动”主题**

### 使用方法
1. 下载这些文件的压缩包：点击 About 左边的 Code 按钮（一般是绿色的），然后点击“Download ZIP”

2. 打开火狐浏览器，在地址栏输入`about:config`，进去搜`stylesheets`，把`toolkit.legacyUserProfileCustomizations.stylesheets`设为`true`

3. 地址栏输`about:profiles`，找到有标注“正在使用此配置文件”的配置文件，之后点击“根目录”那一栏的“打开文件夹”，在文件夹里找到`chrome`文件夹（没有的话就创建一个）

>
>也可以手动导航到配置文件根目录：`[系统盘]\Users\[当前用户名]\AppData\Roaming\Mozilla\Firefox\Profiles\[配置文件ID]`
>
>注意AppData是一个隐藏文件夹
>

4. 将之前的压缩包解压到chrome文件夹（应该不用教吧，毕竟是计算机常识），确保userChrome.css等文件直接位于chrome文件夹下，不要嵌套文件夹

5. 彻底重启火狐浏览器

### 声明
<p>文件 <code>./styles/appbutton_popup_icons.css</code> 的代码来自 <a href="https://github.com/aris-t2/customcssforfx">CustomCSSforFx</a> 项目，该项目具有  <a href="https://www.gnu.org/licenses/gpl-3.0.md">GPLv3</a> /  <a href="https://mozilla.org/MPL/2.0/"> MPLv2</a> 双重许可，这里选择 MPLv2 对该文件进行单文件许可。根据 MPLv2 的要求，在该文件的头部添加了许可声明。</p>
<p>其他文件均采用 MIT 许可证，详见根目录下的 LICENSE 文件。</p>
