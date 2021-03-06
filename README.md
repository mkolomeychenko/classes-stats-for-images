<div align="center" markdown> 



# Collection test


<a data-key="sly-embeded-video-link" href="https://www.youtube.com/watch?v=SczzFM2Os_Y" data-video-code="SczzFM2Os_Y">
    <img src="https://camo.githubusercontent.com/5e8c840f0ca410b15847df365375934e840c7b6f5639a694ca21ae9ab49fe8ba/68747470733a2f2f696d672e796f75747562652e636f6d2f76692f53637a7a464d324f735f592f302e6a7067" alt="SLY_EMBEDED_VIDEO_LINK" data-canonical-src="https://img.youtube.com/vi/SczzFM2Os_Y/0.jpg" style="max-width:100%;">
</a>


<a data-key="sly-embeded-video-link" data-video-code="SczzFM2Os_Y" href="https://www.youtube.com/watch?v=SczzFM2Os_Y">
    <img src="https://camo.githubusercontent.com/5e8c840f0ca410b15847df365375934e840c7b6f5639a694ca21ae9ab49fe8ba/68747470733a2f2f696d672e796f75747562652e636f6d2f76692f53637a7a464d324f735f592f302e6a7067" alt="SLY_EMBEDED_VIDEO_LINK" data-canonical-src="https://img.youtube.com/vi/SczzFM2Os_Y/0.jpg" style="max-width:100%;" />
</a>

# Modules

<div style="display: flex" markdown>


<img  data-key="sly-module-link" data-module-slug="supervisely-ecosystem/create-trainset-for-smarttool" src="https://img.icons8.com/fluent/96/000000/fantasy.png" />

<img  data-key="sly-module-link" data-module-slug="supervisely-ecosystem/yolov5/supervisely/serve" src="https://img.icons8.com/fluent/96/000000/fantasy.png" />

<img  data-key="sly-module-link" data-module-slug="supervisely-ecosystem/nn-image-labeling/annotation-tool" src="https://img.icons8.com/fluent/96/000000/fantasy.png" />



</div>



<p align="center">

  <a href="#overview">Overview</a> •
  <a href="#How-To-Run">How To Run</a> •
  <a href="#Explanation">Explanation</a>
</p>

<img src="https://i.imgur.com/cISE5uw.png"/>

[![](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://supervise.ly/slack) 
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/supervisely-ecosystem/classes-stats-for-images)
[![views](https://app.supervise.ly/public/api/v3/ecosystem.counters?repo=supervisely-ecosystem/classes-stats-for-images&counter=views&label=views&123)](https://supervise.ly)
[![used by teams](https://app.supervise.ly/public/api/v3/ecosystem.counters?repo=supervisely-ecosystem/classes-stats-for-images&counter=downloads&label=used%20by%20teams&123)](https://supervise.ly)
[![runs](https://app.supervise.ly/public/api/v3/ecosystem.counters?repo=supervisely-ecosystem/classes-stats-for-images&counter=runs&label=runs&123)](https://supervise.ly)

</div>

## Overview 

Data Exploration for Segmentation and Detection tasks is underestimated by many researchers. The accuracy of your models highly depends on how good you understand data. 

This app **"Classes Stats for Images"** generates report with detailed general and per image statistics for all classes in images project. It allows to see big picture as well as shed light on hidden patterns and edge cases (see <a href="#how-to-use">How to use</a> section).


## How To Run

### Step 1: Run from context menu of project / dataset

Go to "Context Menu" (images project or dataset) -> "Report" -> "Classes stats for images"

<img src="https://i.imgur.com/dGGzVsm.png" width="600"/>

### Step 2: Configure running settings

Choose the percentage of images that should be randomly sampled. By default all images will be used. And then press "Run" button. In advanced settings you can change agent that will host the app and change version (latest available version is used by default).

<img src="https://i.imgur.com/lI6jenf.png" width="400"/>




<a data-key="sly-embeded-video-link" data-video-code="SczzFM2Os_Y" href="https://www.youtube.com/watch?v=SczzFM2Os_Y">
    <img src="https://camo.githubusercontent.com/5e8c840f0ca410b15847df365375934e840c7b6f5639a694ca21ae9ab49fe8ba/68747470733a2f2f696d672e796f75747562652e636f6d2f76692f53637a7a464d324f735f592f302e6a7067" alt="SLY_EMBEDED_VIDEO_LINK" data-canonical-src="https://img.youtube.com/vi/SczzFM2Os_Y/0.jpg" style="max-width:100%;" />
</a>



# Modules

<div style="display: flex" markdown>


<img  data-key="sly-module-link" data-module-slug="supervisely-ecosystem/create-trainset-for-smarttool" src="https://img.icons8.com/fluent/96/000000/fantasy.png" />

<img  data-key="sly-module-link" data-module-slug="supervisely-ecosystem/yolov5/supervisely/serve" src="https://img.icons8.com/fluent/96/000000/fantasy.png" />

<img  data-key="sly-module-link" data-module-slug="supervisely-ecosystem/nn-image-labeling/annotation-tool" src="https://img.icons8.com/fluent/96/000000/fantasy.png" />



</div>


<div style="display: flex" markdown>


[![SLY_MODULE_LINK](https://img.icons8.com/fluent/96/000000/fantasy.png)](supervisely-ecosystem/create-trainset-for-smarttool)

[![SLY_MODULE_LINK](https://img.icons8.com/fluent/96/000000/fantasy.png)](supervisely-ecosystem/yolov5/supervisely/serve)

[![SLY_MODULE_LINK](https://img.icons8.com/fluent/96/000000/fantasy.png)](supervisely-ecosystem/nn-image-labeling/annotation-tool)


</div>

### Step 3:  Open app

Once app is started, new task appear in workspace tasks. Monitor progress from both "Tasks" list and from application page. To open report in a new tab click "Open" button. 

<img src="https://i.imgur.com/WW4Kacc.png"/>

App saves resulting report to "Files": `/reports/classes_stats/{USER_LOGIN}/{WORKSPACE_NAME}/{PROJECT_NAME}.lnk`. To open report file in future use "Right mouse click" -> "Open".

## Explanation

### Per Image Stats
<img src="https://i.imgur.com/9Hl78Lg.png"/>

Columns:
* `IMAGE ID` - image id in Supervisely Instance
* `IMAGE` - image name with direct link to annotation tool. You can use table to find some anomalies or edge cases in your data by sorting different columns and then quickly open images with annotations to investigate deeper. 
* `HEIGHT`, `WIDTH` - image resolution in pixels
* `CHANNELS` - number of image channels
* `UNLABELED` - percentage of pixels (image area)

Columns for every class:
* <img src="https://i.imgur.com/tyDf3qi.png" width="100"/> - class area (%)
* <img src="https://i.imgur.com/1EquheL.png" width="100"/> - number of objects of a given class (%)

### Per Class Stats

<img src="https://i.imgur.com/ztE4BCG.png"/>

* `CLASS NAME`
* `IMAGES COUNT` - total number of images that have at least one object of a given class
* `OBJECTS COUNT` - total number of objects of a given class
* `AVG CLASS AREA PER IMAGE (%)` -

```
              the sum of a class area on all images               
 -------------------------------------------------------------- 
 the number of images with at least one object of a given class 
```
 
* `AVG OBJECTS COUNT PER IMAGE (%)` - 
```
              total number of class objects               
 -------------------------------------------------------------- 
 the number of images with at least one object of a given class 
```

### Histogram: AVG AREA / AVG OBJECTS COUNT

<img src="https://i.imgur.com/6LXoXHH.png"/>

Histogram view for two metrics from previous chapter: `AVG CLASS AREA PER IMAGE (%)` and `AVG OBJECTS COUNT PER IMAGE (%)`

### Images Count With / Without Class

<img src="https://i.imgur.com/veerIHk.png"/>

### TOP-10 Image Resolutions

<img src="https://i.imgur.com/UwrkTBf.png"/>
