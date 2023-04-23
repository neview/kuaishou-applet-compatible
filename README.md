

## uniapp 转快手小程序的兼容问题


### Hbuilder x 编译快手小程序时一直再等待，没有响应任何东西
```
把项目里的条件注释代码删掉
```

### getLocation:fail 小程序未在AppConfig中注册权限
```
添加一下配置信息
"mp-kuaishou": {
    "permission": {
      "scope.userLocation": {
        "desc": "你的位置信息将用于小程序位置接口的效果展示"
      }
    }
```
### 使用 button open-type="share" 组件时，有灰色边框 
```
给 button 添加 box-shadow:none 属性
```

### 文字超出显示省略号 
```
overflow: hidden;
text-overflow: ellipsis;
-webkit-line-clamp: 1;
-webkit-box-orient: vertical;
```

### scroll-view 区域不能滑动
```
去掉 overflow: hidden
```

### scroll-view 隐藏滚动条
```
::-webkit-scrollbar {
  width: 0;
  height: 0;
  color: transparent;
}
```