# 音乐

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
