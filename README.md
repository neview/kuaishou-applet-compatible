

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
