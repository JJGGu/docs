# 图表区块

图表区块是一个用于组织多个图表的面板。

## 添加区块

点击“添加区块” (Add block) - “图表” (Charts)，可以创建可以空白的图表区块。

![](https://static-docs.nocobase.com/790faf0a126e4ffcc3ff976818325cfd.png)

在图表区块中点击“添加区块” (Add block) - “图表” (Chart)，选择对应的数据表 (Collection), 可以创建和配置图表。有查看权限的数据表才可以用于配置图表，否则将会在选项中被隐藏。

![](https://static-docs.nocobase.com/93ed2fada2478fba1b243d8705717a34.png)

## 区块设置

![](https://static-docs.nocobase.com/202409022042315.png)

- 编辑区块标题 - 可以为区块中的多个图表取一个标题。
- 显示背景 - 是否显示图表区块的背景色。
- 显示内边距 - 是否显示图表区块的内边距。

其中背景和内边距的设置，在区块中只有一个图表时，或者在移动端等场景下，有助于让样式看起来更加舒适。

<img src="https://static-docs.nocobase.com/202404192011039.png"/>

图表区块中的图表可以像普通区块一样，在图表区块中，自由拖拽和组织。

- 点击“配置” (Configure) 按钮，可以修改当前图表的配置。
- 点击“复制” (Duplicate) 按钮，可以快速复制当前图表。
- 点击“删除” (Delete) 按钮，可以删除当前图表。

## 配置区块操作

:::warning{title=提示}
配置操作功能适用于 `v1.4.0-alpha` 版本以后添加的图表区块。
:::

### 刷新和自动刷新

图表区块支持配置刷新按钮，点击刷新区块内的所有图表。

![](https://static-docs.nocobase.com/202409022051107.png)

在配置模式下，点击刷新按钮的设置，可以配置自动刷新间隔，对区块内的所有图表生效。在这个地方配置的自动刷新间隔默认对所有进入页面的用户生效。

![](https://static-docs.nocobase.com/202409022054189.png)

用户在使用的时候也可以通过右侧的按钮修改自动刷新间隔，此处的修改仅在当前生效，页面刷新之后设置会被重置。

![](https://static-docs.nocobase.com/202409022056097.png)

## 配置图表操作

:::info{title=提示}
单个图表上配置的操作按钮，在鼠标进入时才会显示，离开则会自动隐藏。
:::

### 刷新和自动刷新

单个图表上同样支持配置刷新按钮，用法和区块上的刷新按钮一致，对当前图表生效。

![](https://static-docs.nocobase.com/202409022101033.png)

:::info{title=提示}

- 如果图表区块和单个图表上都配置了自动刷新间隔，以图表自身配置的自动刷新间隔为准。
- 如果图表区块上配置了自动刷新间隔，单个图表禁用了自动刷新或未配置刷新按钮，则会沿用图表区块上的设置的自动刷新间隔。
  :::