# 音乐

#### 1.音乐歌单 https://api.hibai.cn/
* API接口在线DEMO： https://api.hibai.cn/api/demo/index  
  @ method : post  
  @ param: {"TransCode":"020111","OpenId":"Test","Body":{"SongListId":"141998290"}}
  ```
  $.ajax({
            type: "POST",
            url: url,
            dataType: 'json',
            data: JSON.parse(param),
            success: function(result){
				$("#result").val(JSON.stringify(result));
                return false;
            },
            error: function(request) {
                alert("Connection error");
                return false;
            }
        });
  ```


#### 搜歌API
```
http://mobilecdn.kugou.com/api/v3/search/song?format=jsonp&keyword=%E4%BB%99%E5%89%91&page=1&pagesize=10&showtype=1&callback=kgJSONP238513750
```

### 百度音乐API
```
@ method: get
@ param: 
  version   5.6.5.0    //版本
  query   七里香//关键字
  method  baidu.ting.search.catalogSug//method
  fromandroid    //平台
  formatjson   //format格式
  
http://tingapi.ting.baidu.com/v1/restserver/ting?from=android&version=5.6.5.0&method=baidu.ting.search.catalogSug&format=json&query=%E4%B8%83%E9%87%8C%E9%A6%99
```
- 关键字搜索（包括歌曲，专辑，歌手，伴奏）
```
http://tingapi.ting.baidu.com/v1/restserver/ting?from=android&version=5.6.5.0&method=baidu.ting.search.merge&format=json&query=%E4%B8%83%E9%87%8C%E9%A6%99&page_no=1&page_size=50&type=-1&data_source=0&use_cluster=1 

参数：（下面应该很容易懂，就不具体解释了）get

version     5.6.5.0
method   baidu.ting.search.merge
format   json
query    七里香
page_no  1
page_size 50
type        -1
data_source  0
use_cluster  1
```
- 获取专辑详情：
```
http://tingapi.ting.baidu.com/v1/restserver/ting?from=android&version=5.6.5.0&method=baidu.ting.album.getAlbumInfo&format=json&album_id=67909

参数：

from  android
version   5.6.5.0
method    baidu.ting.album.getAlbumInfo
format    json
album_id  67909

```

### 网易云音乐平台的音乐接口：
```
搜索歌曲API：

  请求方式：post

  请求地址：http://music.163.com/api/search/get/web?csrf_token=

  请求数据：hlpretag=&hlposttag=&s=搜索歌曲名或歌手名&type=1&offset=0&total=true&limit=返回数据条数

  请求头部：（仅供参考）数组形式

  'Host: music.163.com',

  返回数据：json数据格式，这里就不讲了。

获取歌曲歌词：

  请求方式：get

  请求地址：http://music.163.com/api/song/lyric?

  请求数据：os=pc&id=歌曲id&lv=-1&kv=-1&tv=-1

  返回数据：返回json类型lyric歌曲歌词数据。

获取歌曲直链地址：

  请求方式：get

  请求地址：http://music.163.com/api/song/detail/?

  请求数据：id=歌曲id&ids=%5B歌曲id%5D

  返回数据：返回json类型歌曲文件信息。
```


## 参考地址
* https://www.cnblogs.com/youlixishi/p/6132025.html

### APlayer

* https://github.com/MoePlayer/APlayer
* 在线LRC歌词编辑器: https://github.com/MoeFE/Lyric
