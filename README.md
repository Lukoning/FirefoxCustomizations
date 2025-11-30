# FirefoxCustomizations
本人定制火狐使用的CSS等，适用于Windows系统

<img width="1149" height="757" alt="效果预览" src="https://github.com/user-attachments/assets/a4925dd8-1b1d-4c38-8e99-7d3faaeae4ff" />

由于个人喜好，安装后会自动禁止使用新版配置文件管理器（about:profilemanager），如不喜欢可以在安装后关闭该项功能。

### 使用前建议
打开火狐浏览器，在地址栏输入`about:config`，搜索并设置以下首选项：
<p>
<code>browser.tabs.allow_transparent_browser</code><br>
<code>browser.theme.native-theme</code><br>
<code>widget.non-native-theme.use-theme-accent</code><br>
<code>widget.windows.mica</code><br>
将以上首选项设为<code>true</code>（也就是启用状态）<br><br>
将<code>widget.windows.mica.popups</code>设为<code>2</code><br>
将<code>widget.windows.mica.toplevel-backdrop</code>设为<code>1</code>（ 0 为 MicaAlt [深色云母]，1 为 Mica [云母]，2 为 Acrylic [亚克力]）<br>
将<code>browser.tabs.tabMinWidth</code>设为<code>105</code>（标签页最小宽度，可根据个人喜好修改）<br>
</p>

**不建议使用非默认“系统主题—自动”主题**

如想更换其他主题，建议禁用 widget.windows.mica 。

### 安装方法
1. 下载压缩包：点击右侧栏的“Releases”，找到最新版，点击下面的“Assets”，然后下载“Source code (zip)”

2. 打开火狐浏览器，在地址栏输入`about:config`，进去搜`stylesheets`，把`toolkit.legacyUserProfileCustomizations.stylesheets`设为`true`

3. 地址栏输`about:profiles`，找到有标注“正在使用此配置文件”的配置文件，之后点击“根目录”那一栏的“打开文件夹”，在文件夹里找到`chrome`文件夹（没有的话就创建一个）

>
>也可以手动导航到配置文件根目录：`[系统盘]\Users\[当前用户名]\AppData\Roaming\Mozilla\Firefox\Profiles\[配置文件ID]`
>
>注意AppData是一个隐藏文件夹
>

4. 将之前的压缩包解压到chrome文件夹（应该不用教吧，毕竟是计算机常识），确保userChrome.css这一层的文件和文件夹直接位于chrome文件夹下，不要嵌套其他文件夹

5. 彻底重启火狐浏览器

### 配置

使用 about:config 进行配置

目前提供以下首选项：
<p>boolean: <code>lkn.css.do-not-block-new-profile-management-feature</code> - 不禁用新版配置文件管理器（默认禁用）</p>

### 声明
<p>文件 <code>./styles/appbutton_popup_icons.css</code> 的代码来自 <a href="https://github.com/aris-t2/customcssforfx">CustomCSSforFx</a> 项目，该项目具有  <a href="https://www.gnu.org/licenses/gpl-3.0.md">GPLv3</a> /  <a href="https://mozilla.org/MPL/2.0/"> MPLv2</a> 双重许可，这里选择 MPLv2 对该文件进行单文件许可。根据 MPLv2 的要求，在该文件的头部添加了许可声明。</p>
<p>其他文件均采用 MIT 许可证，详见根目录下的 LICENSE 文件。</p>
