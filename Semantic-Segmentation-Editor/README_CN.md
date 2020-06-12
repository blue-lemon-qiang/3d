# 🐣 语义分割编辑器 (待孵化) 🐣

<br>

[![文档更新时间](https://img.shields.io/badge/更新时间-2020%2F03%2F26-darkorchid.svg?style=for-the-badge&logo=codacy&cacheSeconds=3600)]()
[![文档语言-简体中文](https://img.shields.io/badge/文档语言-简体中文-coral.svg?style=for-the-badge&logo=microsoft-word&cacheSeconds=3600)](./README_CN.md)
[![文档语言-英文](https://img.shields.io/badge/文档语言-英文-mediumpurple.svg?style=for-the-badge&logo=microsoft-word&cacheSeconds=3600)](./README.md)
[![开放源码](https://img.shields.io/badge/开放源码-%E2%9D%A4-brightgreen.svg?style=for-the-badge&logo=conekta&cacheSeconds=3600)]()
[![GitHub Repo Size in Bytes](https://img.shields.io/github/repo-size/eklowlabs/Semantic-Segmentation-Editor.svg?style=for-the-badge&logo=adobe-creative-cloud&cacheSeconds=3600)]()
[![GitHub Release](https://img.shields.io/github/release/eklowlabs/Semantic-Segmentation-Editor.svg?style=for-the-badge&cacheSeconds=3600)]()
[![编程语言-React](https://img.shields.io/badge/编程语言-React-blue.svg?style=for-the-badge&logo=react&logoColor=white&cacheSeconds=3600)]()
[![Github组织-GeekParkHub](https://img.shields.io/badge/Github组织-geekparkhub-blue.svg?style=for-the-badge&logo=microsoft-teams&logoColor=white&cacheSeconds=3600)](https://github.com/geekparkhub)
[![Github组织-AiParkHub](https://img.shields.io/badge/Github组织-aiparkhub-magenta.svg?style=for-the-badge&logo=microsoft-teams&logoColor=white&cacheSeconds=3600)](https://github.com/aiparkhub)
[![Github组织-EklowLabs](https://img.shields.io/badge/Github组织-eklowlabs-coral.svg?style=for-the-badge&logo=microsoft-teams&logoColor=white&cacheSeconds=3600)](https://github.com/eklowlabs)
[![网络站点-EklowLabs](https://img.shields.io/badge/网络站点-EklowLabs-yellow.svg?style=for-the-badge&logo=github&cacheSeconds=3600)](https://github.com/eklowlabs)
[![极客开发者-jeep711](https://img.shields.io/badge/极客开发者-jeep711-azure2.svg?style=for-the-badge&logo=opsgenie&cacheSeconds=3600)](https://github.com/jeep711)

<br>

<div align="center">
<img src="docs/resource/group_sign/eklowlabs_organization_sign.svg" width="650px" alt="EklowLabs-Organization" title="EklowLabs-Organization">
<img src="docs/resource/group_sign/aiparkhub_organization_sign.svg" width="550px" alt="AiParkHub-Organization" title="AiParkHub-Organization">
</div>
<br>


- **埃克洛实验室 | 通过为代码复用与延展构建完美体系 让世界变得更加美好**
- **`Official Public Email`**
- Organization Email：<aiparkhub@outlook.com> —— <geekparkhub@outlook.com> —— <hackerparkhub@outlook.com>  —— <eklowlabs@outlook.com>
- Developer Email：<jeep711.home.@gmail.com> —— <jeep-711@outlook.com>
- System Email：<systemhub-711@outlook.com>
- Service Email：<servicehub-711@outlook.com>


## 1. 前言
#### 向所有科技领域的贡献者致敬

### 1.1 概述
> [语义分割编辑器](https://github.com/eklowlabs/Semantic-Segmentation-Editor)是在研究自动驾驶背景下进行研发, 由`Eklow Labs`基于Web标签工具深度挖掘构建的强大轻量级图像语义分割开源项目;

### 1.2 功能亮点
> 它将用于创建(2D和3D)图像分割AI训练数据集, 该工具它持图像格式(.jpg或.png)和点云格式(.pcd)二进制文件;

#### 1.2.1 位图图像编辑器
> 位图图像 编辑之前
> 
> ![DEMO: Bitmap editor](docs/resource/demo/before_image_segmentation.jpg)

> 位图图像 编辑之后
> 
> ![DEMO: Bitmap editor](docs/resource/demo/after_image_segmentation-2.jpg)


#### 1.2.2 PCD点云编辑器
![DEMO: PCD point cloud editor](docs/resource/demo/pcd_point_cloud.jpg)


## 2. 项目树形结构
```
.
├── LICENSE
├── README.md
├── README_CN.md
├── client
│   ├── jsSetExtensions.js
│   ├── layout.css
│   ├── main.html
│   ├── main.js
│   ├── main.less
│   ├── rc-slider.less
│   ├── routes.jsx
│   └── tippy.css
├── docs
│   └── resource
│       ├── demo
│       │   ├── after_image_segmentation-2.jpg
│       │   ├── after_image_segmentation.jpg
│       │   ├── before_image_segmentation.jpg
│       │   └── pcd_point_cloud.jpg
│       ├── group_sign
│       │   ├── aiparkhub_organization_sign.svg
│       │   └── eklowlabs_organization_sign.svg
│       └── private
│           └── samples
│               ├── bitmap_labeling.jpg
│               └── pointcloud_labeling.pcd
├── imports
│   ├── common
│   │   ├── MapSet.js
│   │   ├── SseBottomBar.jsx
│   │   ├── SseBranding.jsx
│   │   ├── SseClassChooser.jsx
│   │   ├── SseConfirmationDialog.jsx
│   │   ├── SseDataManager.js
│   │   ├── SseGlobals.jsx
│   │   ├── SseMsg.js
│   │   ├── SsePopup.jsx
│   │   ├── SseSetOfClasses.js
│   │   ├── SseText.jsx
│   │   ├── SseTheme.js
│   │   └── SseToolbar.jsx
│   ├── editor
│   │   ├── 2d
│   │   │   ├── SseApp2d.jsx
│   │   │   ├── SseEditor2d.jsx
│   │   │   ├── SseGeometry.jsx
│   │   │   ├── SseLayers.jsx
│   │   │   ├── SseSliderPanel.jsx
│   │   │   ├── SseToolbar2d.jsx
│   │   │   ├── SseTooltips2d.jsx
│   │   │   ├── SseUndoRedo2d.js
│   │   │   ├── SseZoom.js
│   │   │   └── tools
│   │   │       ├── SseCutTool.js
│   │   │       ├── SseFloodPanel.jsx
│   │   │       ├── SseFloodTool.js
│   │   │       ├── SsePointerTool.js
│   │   │       ├── SsePolygonTool.js
│   │   │       ├── SseRectangleTool.js
│   │   │       ├── SseTool.js
│   │   │       └── magicwand.js
│   │   ├── 3d
│   │   │   ├── GradientBoxHelper.js
│   │   │   ├── SseApp3d.jsx
│   │   │   ├── SseCameraToolbar.jsx
│   │   │   ├── SseEditor3d.jsx
│   │   │   ├── SseObjectToolbar.jsx
│   │   │   ├── SsePCDLoader.js
│   │   │   ├── SseToolbar3d.jsx
│   │   │   ├── SseTooltips3d.jsx
│   │   │   └── tools
│   │   │       ├── OrbitControls.js
│   │   │       ├── Sse3dCircleSelector.js
│   │   │       ├── Sse3dLassoSelector.js
│   │   │       ├── Sse3dRectangleSelector.js
│   │   │       └── Sse3dSelector.js
│   │   └── SseEditorApp.jsx
│   └── navigator
│       ├── SseAllAnnotated.jsx
│       ├── SseImageThumbnail.jsx
│       ├── SseNavigatorApp.jsx
│       ├── SseNavigatorMenu.jsx
│       └── SseNavigatorToolbar.jsx
├── lib
│   └── collections.js
├── package-lock.json
├── package.json
├── public
│   ├── SseDataWorker.js
│   ├── pcl_horz_large_neg.png
│   └── pcl_vert_large_neg.png
├── server
│   ├── SseDataWorkerServer.js
│   ├── api.js
│   ├── config.js
│   ├── files.js
│   └── main.js
└── settings.json

18 directories, 76 files
```

## 3. 如何使用
### 3.1 克隆工程
``` bash
git clone https://github.com/eklowlabs/Semantic-Segmentation-Editor.git
```

### 3.2 安装 Meteor (OSX or Linux) 
```shell
curl https://install.meteor.com/ | sh
```
或 下载  [Meteor Windows Installer](http://www.meteor.com/install)


### 3.3 启动应用程序
```shell
cd Semantic-Segmentation-Editor-x.x.x
meteor npm install
meteor npm start
```

默认情况下编辑器将在 `http://localhost:3000` 运行;


### 3.4 (可选项) 编辑 `settings.json`
 
> 默认情况下，图像从 <code>your_home_dir/sse-images</code> 和pointcloud二进制分段数据存储在 <code>your_home_dir/sse-internal</code>.
> 你可以通过修改在settings.json中配置这些文件夹 <code>images-folder</code> 和 <code>internal-folder</code> 属性. 在Windows上，使用 '/' separators, example <code>c:/Users/john/images</code>

### 3.5 配置文件 `settings.json`
``` bash
{
  "configuration": {
    "images-folder": "/xxx/images", // 包含图像和PCD文件的根文件夹
    "internal-folder": "/xxx/pointcloud_data" // 分割数据（仅3D）将存储在此文件夹中
  },
  // The different sets of classes available in the tool
  // For object classes, only the 'label' field is mandatory
  // The icon field can be set with an icon from the mdi-material-ui package
  "sets-of-classes": [
    {
      "name": "Cityscapes", "objects": [
      {"label": "VOID", "color": "#CFCFCF"},
      {"label": "Road", "color": "#804080", "icon": "Road"},
      {"label": "Sidewalk", "color": "#F423E8", "icon": "NaturePeople"},
      {"label": "Parking", "color": "#FAAAA0", "icon": "Parking"},
      {"label": "Rail Track", "color": "#E6968C", "icon": "Train"},
      {"label": "Person", "color": "#DC143C", "icon": "Walk"},
      {"label": "Rider", "color": "#FF0000", "icon": "Motorbike"},
      {"label": "Car", "color": "#0000E8", "icon": "Car"}
    },
    { ... }
  ]
}
```
f
### 3.6 使用位图图像编辑器
#### 3.6.1 多边形绘图工具 (P)
- 单击和/或拖动以创建点;
- ESC按键以相反的顺序删除最后创建的点;
- 拖动鼠标指针或按住Shift键即可创建复杂的多边形, 而无需为每个点单击;
- 回车按键或双击第一个点以关闭多边形;
  
  
#### 3.6.2 魔术工具 (A)
- 使用对比度阈值检测自动创建多边形;
- 此工具仅可用于绘制边缘锐利对比的对象的轮廓 (例如: 天空, 车道标记);
- 在要勾勒轮廓的区域内单击, 然后调整右侧的任何滑块以调整结果;
- 以回车按键验证结果;

#### 3.6.3 操作工具 (Alt)
- 选择, 移动点并将其添加到现有多边形;
- 在多边形内部单击以将其选中;
- 单击一个点将其选中;
- 在多个点周围绘制套索以选择它们;
- 用鼠标拖动一个点将其移动;
- 按住Shift键可分离属于多个多边形的点;
- 单击多边形的线以创建新点, 然后拖动新创建的点以将其放置;

#### 3.6.4 切割/扩张工具 (C)
- 修改现有多边形的形状;
- 选择要修改的多边形;
- 在多边形的轮廓上画一条开始和结束线;
- 新行替换起点和终点之间的现有路径;
- 结果形状始终是最大的形状;

#### 3.6.5 连续多边形工具 (F)
- 轻松创建连续的多边形;
- 使用多边形绘图工具开始一个新的多边形;
- 通过捕捉到要解决的多边形的轮廓来创建起点;
- 通过捕捉到另一个轮廓来创建终点, 这时必须具有一条与一个或多个现有多边形相交的直线;
- 按F键一次或几次以选择要使用的解决方法;



### 3.7 使用点云编辑器
- 鼠标左键：围绕当前焦点旋转点云(默认情况下, 点云的中心), 单击单个点将其添加到当前选择中;
- 鼠标滚轮：放大/缩小;
- 鼠标中键(或Ctrl + Click)更改摄像机的目标;
- 鼠标右键: 用于根据当前选择工具和选择模式同时选择多个点;


### 3.8 支持 PCD
- 支持的输入PCD格式: ASCII, 二进制和二进制压缩
- 支持输入字段: `x`，`y`，`z`，`label`(可选整数), `rgb`(可选整数);
- 输出的PCD格式为ASCII, 带有字段 `x`, `y`, `z`, `label`, `object`  和 `rgb` (如果可供使用的话)

### 3.9 API
- <code>/api/listing</code>: 列出所有带注释的图像;
- <code>/api/json/[PATH_TO_FILE]</code>: (仅限2D) 获取该文件的多边形和其他数据;
- <code>/api/pcdtext/[PATH_TO_FILE]</code>: (仅限3D) 使用2个附加元素获取pcd文件的标签;
列: <code>标签</code>
和 <code>对象</code>
-  <code>/api/pcdfile/[PATH_TO_FILE]</code>: (仅限3D)相同, 但返回为"纯文本/文本"附件文件下载;


## 4. 开源协议
 [MIT License](./LICENSE)
 
 ---------
