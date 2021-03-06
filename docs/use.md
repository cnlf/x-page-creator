# 使用文档

## 入口

![创建页面](@/assets/images/document/1.png)

通过管理平台【页面搭建平台】>【模板列表管理】界面，点击【新增】按钮，进入新版搭建系统直接创建页面。

![编辑页面](@/assets/images/document/1-2.png)

也可以在列表页面双击进入页面详情，点击【编辑】按钮，进入搭建系统编辑页面或模板。

> 请注意新版页面搭建系统上线后，只允许使用新系统创建页面，并保留了之前老系统创建的页面的编辑功能。

## 编辑界面

![默认页面编辑界面](@/assets/images/document/2.png)

新增进入创建界面，默认为创建PC页面，可以在右上角切换为移动页面。当编辑内容为模板时，不允许切换类型（PC/移动）。

![移动页面编辑界面](@/assets/images/document/2-1.png)

![移动机型尺寸选择](@/assets/images/document/2-2.png)

移动界面可选择机型尺寸，在编辑时实时查看当前编辑内容在各种不同机型的效果。

> 注意：这里选择机型只是提供尺寸参考，实际效果应当以实际设备查看为准。

----

**【编辑模式】** 

页面处于编辑模式时，可以在编辑区域进行编辑操作，编辑区域呈现透明背景模式，容器组件会显示容器标识，并且顶部15px内边距和黄色边框。

- 按住键盘`Ctrl`并鼠标单击组件，聚焦当前组件，显示蓝色外边框聚焦效果；

- 双击组件时聚焦并弹出右侧编辑面板；

- 在不同组件右键点击时显示不同的操作选项菜单；

- 拖拽左侧面板组件到编辑区域的组件上方时，相关组件会显示阴影效果：外放阴影表明将于后面创建相邻组件；内放阴影表明将于其内底部创建子组件；

- 拖拽编辑区域内部组件时，可以改变组件间嵌套关系或相邻关系，阴影效果与拖拽创建组件类似；

- 也可使用快捷键进行快捷操作。

**【预览模式】**

页面最大化，同时隐藏编辑相关面板，显示真实页面效果。移动端可选择机型尺寸进行查看。

----

![图片素材管理](@/assets/images/document/2-3.png)

**【图片素材】** 界面使用操作方式与老系统基本一致；

![模板管理](@/assets/images/document/2-4.png)

**【模板】** 管理界面显示的模板列表只展示与当前页面类型（PC/移动）相同的模板。选中模板后，可应用到当前编辑内容，如果是属于自己创建的模板也可以对模板进行编辑。

![应用模板询问框](@/assets/images/document/2-5.png)

> 注意：应用模板时，会有询问框提示是否同时将页面基础信息也应用到当前编辑页面或模板，如果要取消模板应用，应该点击右上角关闭按钮。如果操作失误而应用了模板，想要撤销可以右键撤销，页面内容将恢复到应用模板之前。

----

**【基础设置】** 设置界面即设置页面名称和SEO信息，页面和模板都可以设置。

![基础设置](@/assets/images/document/2-6.png)

**【模板设置】** 设置界面即设置模板名称和模板是否可共享，即其他人是否也可以为页面应用该模板。

![模板设置](@/assets/images/document/2-7.png)

----

**【清空】** 清空页面内容，仅为本地操作，误操作时只要没有点击【保存】，可通过右键撤销或者直接F5刷新页面返回清空操作之前的状态。

**【保存】** 将当前页面或模板编辑内容保存到服务器。如果是新创建页面，将会弹出基础设置弹窗，设置页面基础信息后保存到服务器。

**【保存为新模板】** 可以是基于页面也可以是基于模板保存为新模板，弹出模板设置点击保存创建新模板。

### 组件编辑

**【展开】** 可以扩展编辑界面，方便编辑。

**【组件树】** 可以切换显示页面组件树结构，点击树节点以聚焦组件，编辑界面的编辑组件也会切换为当前聚焦组件进行编辑。通过该界面，能够清晰的看到页面组件嵌套关系，注意避免嵌套深度过深。

**【属性编辑】** 通过编辑组件属性，可以实时观察到页面的变化。

## 组件

- 布局组件

- 基础组件

- 高级组件

### 布局组件

布局组件即是一种容器组件，可以包含嵌套其他组件，这里分为根容器、普通容器、定位容器、悬浮容器、行容器、列容器。

#### 根容器

即页面组件树的根节点，一个页面只能包含一个根容器。它不能直接放置一般组件，只能放置**普通容器、行容器、定位容器和悬浮容器**。

可以设置背景。

#### 普通容器

普通容器可以放置**普通容器、行容器、定位容器和其他非容器组件**。

可以设置布局、背景、悬浮效果（移动端无该设置）和动画等样式效果。

#### 行容器

行容器即以单独一行呈现的容器，**只允许放置列容器**，采用了**flex布局**模式。内部列容器只允许横向排列，超出宽度时可以设置横向滚动。

可以设置布局、背景、悬浮效果和动画等样式效果。

#### 列容器

列容器即行容器的子组件且也只能作为行容器的子组件。可以放置**普通容器、行容器、定位容器和其他非容器组件**。

可以设置布局、背景、悬浮效果和动画等样式效果。

#### 定位容器

定位容器即可以基于父容器进行定位的容器，可以拖拽组件头部定位，并不限于定位到父容器之外。

可以放置**普通容器、行容器、定位容器和其他非容器组件**。

可以设置定位、布局、背景、悬浮效果和动画等样式效果。

#### 悬浮容器

悬浮容器基于视口定位，只能作为根容器的子组件，可以拖拽组件头部定位。

可以放置**普通容器、行容器、定位容器和其他非容器组件**。

可以设置定位、布局、背景、悬浮效果和动画等样式效果。

### 基础组件

基础组件非常灵活，可以通过多种基础组件组装成为一个复杂的模块，之后可通过复制在当前页面重复利用，或保存为模板来跨页面跨模板重复利用。

### 高级组件

一般常见常用的模块结构，可以直接使用的有一定复杂度的模块，通过简单设置，可以更高效的创建页面，但灵活度较弱。

后续会陆续开发增加到组件库。

## 缓存历史

- 缓存页面内容。可以通过右键菜单【缓存】或快捷键【Ctrl+S】

- 撤销到上一次缓存记录。可以通过右键菜单【撤销】或快捷键【Ctrl+Z】

## 右键菜单

不同组件会有不同的的右键菜单操作选项。

- **编辑** 编辑当前焦点组件，显示组件编辑面板

- **剪切** 将当前焦点组件从页面中移除到剪贴板中等待粘贴， **注意这里的剪贴板只在当前页面起作用，不可跨页面粘贴**

- **复制** 将当前焦点组件复制到剪贴板中等待粘贴

- **粘贴** 将剪贴板中保存的组件粘贴放置到当前焦点组件，根据组件嵌套规则确定是放置在焦点组件下方还是内部。

<!-- - **缓存** 将当前页面内容缓存到历史记录。这里只是本地缓存，F5刷新页面时，如果当编辑页面是已创建过的页面缓存记录会被重置，建议应该尽量【保存】页面到服务器。 -->

<!-- - **撤销** 将当前页面内容撤销到缓存历史记录中上一次缓存记录。 -->

- **置空** 将当前焦点组件内部子组件清空

- **移除** 将当前焦点组件从页面中移除

- **插入xxx** 在当前焦点组件中插入xxx组件

- **前移** 当前焦点组件在同层级中向前移动一位

- **后移** 当前焦点组件在同层级中向后移动一位

- **置首** 当前焦点组件在同层级中向前置顶

- **置尾** 当前焦点组件在同层级中向后置尾

- **前外移** 当前焦点组件移动到父组件同层级，并置于父组件前方

- **后外移** 当前焦点组件移动到父组件同层级，并置于父组件后方

## 快捷键

- **Ctrl + `** 编辑模式与预览模式间切换

- **Escape** 关闭组件编辑界面

<!-- - **Ctrl + S** 缓存 -->

<!-- - **Ctrl + Z** 撤销 -->

- **Ctrl + S** 保存页面内容

- **Ctrl + 鼠标单击** / **双击** / **右键** 聚焦组件

- **Tab** 切换聚焦组件

- **Shift + Tab** 反向切换聚焦组件

- **Ctrl + C** 复制

- **Ctrl + X** 剪切

- **Ctrl + V** 粘贴

- **Ctrl + Delete** 移除

- **Ctrl + ←/↑** 前移

- **Ctrl + Shift + ←/↑** 置首

- **Ctrl + →/↓** 后移

- **Ctrl + Shift + →/↓** 置尾

- **Ctrl + Alt + ←/↑** 前外移

- **Ctrl + Alt + →/↓** 后外移

## 注意事项

- 移动端组件布局时请注意避免将宽高设置为固定尺寸，因为不同设备的逻辑像素是不一致的，建议尽量使用自适应的宽高。
