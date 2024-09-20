/*
    第18行背景图片自行替换
    第20行模糊度
*/

/* 伪元素 图片模糊 */
.MuiPaper-root.windows.layout {
  position: relative;
  overflow: hidden; /* 防止模糊效果溢出 */
}

.MuiPaper-root.windows.layout::before {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background-image: url(https://cfr2.comety.tech/12324545.png);
  background-size: cover;
  filter: blur(5px);
  /* 你也可以根据需要调整模糊度 */
}

/* 基础页面容器背景 */
.base-page .base-container {
    background-color: rgba(164, 60, 60, 0) !important; /* 半透明: rgba(164, 60, 60, 0.5) */
}

.base-page .base-container.no-padding > section {
    background-color: rgba(164, 60, 60, 0) !important; /* 同上 */
}

/* ---代理--- */
/* 使用更通用的类名，并增加层级来提高选择器的特异性 */
.MuiListItemButton-root.dense.gutters {
    background-color: rgba(244, 237, 237, 0.38) !important; /* #f4eded63 转换为 rgba */
}

.MuiListItemButton-root.dense.gutters.active { /* 假设有 active 状态 */
    background-color: rgba(159, 149, 149, 0.38) !important; /* #9f959563 转换为 rgba */
}

/* ---节点背景--- */
/* 增加特异性并使用更深的背景颜色 */
.MuiListItemButton-root.dense.gutters.node {
    background-color: rgba(39, 39, 39, 0.85) !important; /* 深灰色，减少透明度以加深颜色 */
    color: #000000 !important; /* 确保文字为白色 */
}

.MuiListItemButton-root.dense.gutters.node .node-name,
.MuiListItemButton-root.dense.gutters.node .node-type,
.MuiListItemButton-root.dense.gutters.node .node-latency {
    color: #000000 !important; /* 确保节点内所有文本为白色 */
}

/* ---订阅--- */
/* 使用更通用的选择器，并增加层级 */
.base-page .base-container .MuiBox-root > div {
    background-color: rgba(39, 39, 39, 0.1) !important; /* #bababab8 转换为 rgba */
}

.base-page .base-container .MuiBox-root.another-class > div { /* 替换 .css-xev7gz 为更稳定的类名 */
    background-color: rgba(39, 39, 39, 0) !important;
}

/* ---连接--- */
.connection-class { /* 替换 .css-t4n4qq 为更稳定的类名 */
    background-color: rgba(11, 11, 14, 0.24) !important; /* rgb(11 11 14 / 24%) 转换为 rgba */
}

/* ---规则--- */
.rules-class { /* 替换 .css-16nv95e 为更稳定的类名 */
    background-color: rgba(39, 29, 29, 0.17) !important; /* #271d1d45 转换为 rgba */
}

/* ---设置--- */
.base-page .base-container > section.settings {
    background-color: rgba(255, 255, 255, 0.18) !important; /* #ffffff2b 转换为 rgba */
}

.settings-container .MuiGrid-root {
    background-color: rgba(39, 39, 39, 0.1) !important; /* #413b3b38 转换为 rgba */
}
