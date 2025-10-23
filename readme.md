
# heer-tools

## 介绍
一个基于 UTS 实现的调用鸿蒙原生功能的API

## 安装方法
1. 在uni-app插件市场中搜索并导入heer-tools
2. 重新运行鸿蒙项目
3. 在页面中导入插件

## 代码演示
跳转到鸿蒙拨打电话界面
```vue
<template>
	<view>
		<button @click="appMakeCallHandle">拨打电话</button>
	</view>
</template>

<script setup>
	import {
		appMakeCall
	} from "@/uni_modules/heer-tools"
	function appMakeCallHandle() {
		appMakeCall("13312341234")
	}
</script>
```

## API文档

| 方法名         | 说明      | 参数               | 返回值 |
| ----------- | ------- | ---------------- | --- |
| appMinimize | 最小化返回桌面 | -                | -   |
| appMakeCall | 拨打电话    | tel:string(电话号码) | -   |
