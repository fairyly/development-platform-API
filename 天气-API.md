# 天气

## 和风天气
```
权限             普通用户             认证个人开发者            认证企业开发者
应用数量            1                      3                       5
创建KEY数量        3个/应用              5个/应用                 5个/应用
天气预报数据        3天                   7天                       7天
实况天气数据        -                      有                        有
逐三小时预报数据     -                     有                         有
格点预报数据         -                     有                        有
付费数据免费试用     -                     -                         10天
免费访问量           1000次/天           16700次/天                16700次/天
折扣优惠券           无                  无                         1000元
技术支持            邮件                  邮件                   邮件、电话
专人对接            -                     -                        有
商业授权            -                     -                        -
```

- 1.空气质量数据集合
>包括空气质量实况数据、空气质量未来7天预报以及空气质量未来逐小时预报，   
有权限的用户可通过本接口一次性获取某一地区以上所有空气质量相关数据。

`url`: `https://api.heweather.net/s6/air?location=116.40,39.9&key=`


- 2.常规天气数据集合

>接口包含了3-7天天气预报、实况天气、逐小时天气预报以及生活指数，  
有对应权限的用户可通过访问此接口一次性获取某一地区的上述所有天气数据;  
普通用户通过此接口仅获得3天预报数据，  
认证个人开发者可获取7天预报和24小时内逐3小时预报数据，实况数据以及免费的生活指数，  
有权限的付费用户则可获得对应权限的全部数据,    
本集合接口中，生活指数仅限国内地区，如查询海外城市，则该数据字段将不提供

`url`: `https://free-api.heweather.net/s6/weather?location=116.40,39.9&key=`

- 3.空气质量实况
>环保部1500+个监测站点实时空气质量（AQI）数据，  
以及目前唯一可提供的全国3240个城市的实时空气质量（AQI）数据;  
环保部1500+个监测站点实况数据为免费数据，全国3240个城市实时空气质量指数为付费数据  

普通用户和认证开发者仅可访问全国地级市及地级市所辖的国控站点数据，  
且不支持通过经纬度获取数据（可使用城市名称、ID、IP）

`url`: `https://free-api.heweather.net/s6/air/now?location=116.40,39.9&key=`

- 4.生活指数
>生活指数和生活指数预报包括：穿衣、洗车、感冒、紫外线、运动、舒适度、旅游、空气污染扩散条件

`url`: `https://free-api.heweather.net/s6/weather/lifestyle?location=116.40,39.9&key=`

- 5.日出日落
>可获得全球3-7天日出日落时间  
付费用户若未购买3天（不含）以上的预报数据，则只能获得默认三天的日出日落时间


`url`: `https://free-api.heweather.net/s6/solar/sunrise-sunset?location=116.40,39.9&key=`



- 6.3-10天天气预报
>最长10天天气预报数据，天气预报包含的数据：  
日出日落、月升月落、最高最低温度、天气白天和夜间状况、风力、风速、风向、  
相对湿度、大气压强、降水量、降水概率、露点温度、紫外线强度、能见度等数据  
城市覆盖范围：全球  
大客户可达14天，免费用户获得 3天预报数据，认证开发者可获得7天预报，付费用户可选 3-10天

`url`: `https://free-api.heweather.net/s6/weather/forecast?location=116.40,39.9&key=`



- 7.逐小时天气预报
>未来24-168个小时，逐小时的天气预报数据数据，  
具体包含的数据：温度、天气状况、风力、风速、风向、相对湿度、大气压强、降水概率等。  
城市覆盖范围：全球  
认证开发者可获得24小时内逐三小时的预报数据，付费用户可选择未来24-168小时内逐1小时预报的数据

`url`: `https://free-api.heweather.net/s6/weather/hourly?location=116.40,39.9&key=`

- 8.实况天气
>实况天气即为当前时间点的天气状况以及温湿风压等气象指数，  
具体包含的数据：体感温度、实测温度、天气状况、风力、风速、风向、相对湿度、大气压强、降水量、能见度等。

`url`: `https://free-api.heweather.net/s6/weather/now?location=116.40,39.9&key=`



- 9.热门城市列表
>特殊值：world，返回全球热门城市  
特殊值：cn，返回中国热门城市  
特殊值：overseas，查询海外热门城市（不含中国）

`url`: `https://search.heweather.net/top?group=cn&key=`

- 10.城市搜索
>

`url`: `https://search.heweather.net/find?location=北京&key=`

- 天气状况代码和图标

> [天气状况代码和图标](https://www.heweather.com/documents/condition)

====================================================================

#和风天气天气状况代码和图标

> 更新日期：2018年5月30日，请定期访问[天气状况代码文档页](https://www.heweather.com/documents/condition)以便获取最新的天气状况代码

##天气图标
###版权
和风天气图标采用<a href="https://creativecommons.org/licenses/by-nc/3.0/cn/" title="署名-非商业性使用 3.0 中国大陆 (CC BY-NC 3.0 CN)">署名-非商业性使用 3.0 中国大陆 (CC BY-NC 3.0 CN)</a>许可协议授权
###下载
[图片打包下载](https://cdn.heweather.com/cond-icon-heweather.zip)
###使用
* 图标文件名为天气代码，后缀为.png
* 图标文件名中有字母`n`的，为夜间天气图标，例如[100n.png](https://cdn.heweather.com/cond_icon/100n.png "晴天图标")

##天气代码对照表
| 代码 | 中文 | 英文 | 图标 |
|---|---|---|---|
| 100 | 晴 | Sunny/Clear |[100.png](https://cdn.heweather.com/cond_icon/100.png "晴天图标")|
| 101 | 多云 | Cloudy | [101.png](https://cdn.heweather.com/cond_icon/101.png "多云图标") |
| 102 | 少云 | Few Clouds | [102.png](https://cdn.heweather.com/cond_icon/102.png "少云图标") |
| 103 | 晴间多云 | Partly Cloudy | [103.png](https://cdn.heweather.com/cond_icon/103.png "晴间多云图标") |
| 104 | 阴 | Overcast | [104.png](https://cdn.heweather.com/cond_icon/104.png "阴图标") |
| 200 | 有风 | Windy | [200.png](https://cdn.heweather.com/cond_icon/200.png "有风图标") |
| 201 | 平静 | Calm | [201.png](https://cdn.heweather.com/cond_icon/201.png "平静图标") |
| 202 | 微风 | Light Breeze | [202.png](https://cdn.heweather.com/cond_icon/202.png "微风图标") |
| 203 | 和风 | Moderate/Gentle Breeze | [203.png](https://cdn.heweather.com/cond_icon/203.png "和风图标") |
| 204 | 清风 | Fresh Breeze | [204.png](https://cdn.heweather.com/cond_icon/204.png "清风图标") |
| 205 | 强风/劲风 | Strong Breeze | [205.png](https://cdn.heweather.com/cond_icon/205.png "强风图标") |
| 206 | 疾风 | High Wind, Near Gale | [206.png](https://cdn.heweather.com/cond_icon/206.png "疾风图标") |
| 207 | 大风 | Gale | [207.png](https://cdn.heweather.com/cond_icon/207.png "大风图标") |
| 208 | 烈风 | Strong Gale | [208.png](https://cdn.heweather.com/cond_icon/208.png "烈风图标") |
| 209 | 风暴 | Storm | [209.png](https://cdn.heweather.com/cond_icon/209.png "风暴图标") |
| 210 | 狂爆风 | Violent Storm | [210.png](https://cdn.heweather.com/cond_icon/210.png "狂爆风图标") |
| 211 | 飓风 | Hurricane | [211.png](https://cdn.heweather.com/cond_icon/211.png "飓风图标") |
| 212 | 龙卷风 | Tornado | [212.png](https://cdn.heweather.com/cond_icon/212.png "龙卷风图标") |
| 213 | 热带风暴 | Tropical Storm | [213.png](https://cdn.heweather.com/cond_icon/213.png "热带风暴图标") |
| 300 | 阵雨 | Shower Rain | [300.png](https://cdn.heweather.com/cond_icon/300.png "阵雨图标") |
| 301 | 强阵雨 | Heavy Shower Rain | [301.png](https://cdn.heweather.com/cond_icon/301.png "强阵雨图标") |
| 302 | 雷阵雨 | Thundershower | [302.png](https://cdn.heweather.com/cond_icon/302.png "雷阵雨图标") |
| 303 | 强雷阵雨 | Heavy Thunderstorm | [303.png](https://cdn.heweather.com/cond_icon/303.png "强雷阵雨图标") |
| 304 | 雷阵雨伴有冰雹 | Hail | [304.png](https://cdn.heweather.com/cond_icon/304.png "雷阵雨伴有冰雹图标") |
| 305 | 小雨 | Light Rain | [305.png](https://cdn.heweather.com/cond_icon/305.png "小雨图标") |
| 306 | 中雨 | Moderate Rain | [306.png](https://cdn.heweather.com/cond_icon/306.png "中雨图标") |
| 307 | 大雨 | Heavy Rain | [307.png](https://cdn.heweather.com/cond_icon/307.png "大雨图标") |
| 308 | 极端降雨 | Extreme Rain | [308.png](https://cdn.heweather.com/cond_icon/308.png "极端降雨图标") |
| 309 | 毛毛雨/细雨 | Drizzle Rain | [309.png](https://cdn.heweather.com/cond_icon/309.png "毛毛雨图标") |
| 310 | 暴雨 | Storm | [310.png](https://cdn.heweather.com/cond_icon/310.png "暴雨图标") |
| 311 | 大暴雨 | Heavy Storm | [311.png](https://cdn.heweather.com/cond_icon/311.png "大暴雨图标") |
| 312 | 特大暴雨 | Severe Storm | [312.png](https://cdn.heweather.com/cond_icon/312.png "特大暴雨图标") |
| 313 | 冻雨 | Freezing Rain | [313.png](https://cdn.heweather.com/cond_icon/313.png "冻雨图标") |
| 314 | 小到中雨 | Light to moderate rain | [314.png](https://cdn.heweather.com/cond_icon/314.png "小到中雨图标") |
| 315 | 中到大雨 | Moderate to heavy rain | [315.png](https://cdn.heweather.com/cond_icon/315.png "中到大雨图标") |
| 316 | 大到暴雨| Heavy rain to storm | [316.png](https://cdn.heweather.com/cond_icon/316.png "大到暴雨图标") |
| 317 | 暴雨到大暴雨 | Storm to heavy storm | [317.png](https://cdn.heweather.com/cond_icon/317.png "暴雨到大暴雨图标") |
| 318 | 大暴雨到特大暴雨 | Heavy to severe storm | [318.png](https://cdn.heweather.com/cond_icon/318.png "大暴雨到特大暴雨图标") |
| 399 | 雨 | Rain | [399.png](https://cdn.heweather.com/cond_icon/399.png "雨图标") |
| 400 | 小雪 | Light Snow | [400.png](https://cdn.heweather.com/cond_icon/400.png "小雪图标") |
| 401 | 中雪 | Moderate Snow | [401.png](https://cdn.heweather.com/cond_icon/401.png "中雪图标") |
| 402 | 大雪 | Heavy Snow | [402.png](https://cdn.heweather.com/cond_icon/402.png "大雪图标") |
| 403 | 暴雪 | Snowstorm | [403.png](https://cdn.heweather.com/cond_icon/403.png "暴雪图标") |
| 404 | 雨夹雪 | Sleet | [404.png](https://cdn.heweather.com/cond_icon/404.png "雨夹雪图标") |
| 405 | 雨雪天气 | Rain And Snow | [405.png](https://cdn.heweather.com/cond_icon/405.png "雨雪天气图标") |
| 406 | 阵雨夹雪 | Shower Snow | [406.png](https://cdn.heweather.com/cond_icon/406.png "阵雨夹雪图标") |
| 407 | 阵雪 | Snow Flurry | [407.png](https://cdn.heweather.com/cond_icon/407.png "阵雪图标") |
| 408 | 小到中雪 | Light to moderate snow | [408.png](https://cdn.heweather.com/cond_icon/408.png "小到中雪图标") |
| 409 | 中到大雪 | Moderate to heavy snow | [409.png](https://cdn.heweather.com/cond_icon/409.png "中到大雪图标") |
| 410 | 大到暴雪 | Heavy snow to snowstorm | [410.png](https://cdn.heweather.com/cond_icon/410.png "大到暴雪图标") |
| 499 | 雪 | Snows | [499.png](https://cdn.heweather.com/cond_icon/499.png "雪图标") |
| 500 | 薄雾 | Mist | [500.png](https://cdn.heweather.com/cond_icon/500.png "薄雾图标") |
| 501 | 雾 | Foggy | [501.png](https://cdn.heweather.com/cond_icon/501.png "雾图标") |
| 502 | 霾 | Haze | [502.png](https://cdn.heweather.com/cond_icon/502.png "霾图标") |
| 503 | 扬沙 | Sand | [503.png](https://cdn.heweather.com/cond_icon/503.png "扬沙图标") |
| 504 | 浮尘 | Dust | [504.png](https://cdn.heweather.com/cond_icon/504.png "浮尘图标") |
| 507 | 沙尘暴 | Duststorm | [507.png](https://cdn.heweather.com/cond_icon/507.png "沙尘暴图标") |
| 508 | 强沙尘暴 | Sandstorm | [508.png](https://cdn.heweather.com/cond_icon/508.png "强沙尘暴图标") |
| 509 | 浓雾 | Dense fog | [509.png](https://cdn.heweather.com/cond_icon/509.png "浓雾图标") |
| 510 | 强浓雾 | Strong fog | [510.png](https://cdn.heweather.com/cond_icon/510.png "强浓雾图标") |
| 511 | 中度霾 | Moderate haze | [511.png](https://cdn.heweather.com/cond_icon/511.png "中度霾图标") |
| 512 | 重度霾 | Heavy haze | [512.png](https://cdn.heweather.com/cond_icon/512.png "重度霾图标") |
| 513 | 严重霾 | Severe haze | [513.png](https://cdn.heweather.com/cond_icon/513.png "重度霾图标") |
| 514 | 大雾 | Heavy fog | [514.png](https://cdn.heweather.com/cond_icon/514.png "大雾图标") |
| 515 | 特强浓雾 | Extra heavy fog | [515.png](https://cdn.heweather.com/cond_icon/515.png "特强浓雾图标") |
| 900 | 热 | Hot | [900.png](https://cdn.heweather.com/cond_icon/900.png "热图标") |
| 901 | 冷 | Cold | [901.png](https://cdn.heweather.com/cond_icon/901.png "冷图标") |
| 999 | 未知 | Unknown | [999.png](https://cdn.heweather.com/cond_icon/999.png "未知图标") |


## 参考
- [开发文档](https://www.heweather.com/documents/api/s6/air-all)
- [状态码和错误码](https://www.heweather.com/documents/status-code)
