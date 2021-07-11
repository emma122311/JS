# JS(語法)
換行設定（ word-wrap & word-break）
```
word-break: break-all
//文字強迫換行，太長的英文字，會自動切成兩半。
//參考網址：https://www.puritys.me/docs-blog/article-31-CSS-%E8%AA%9E%E6%B3%95%EF%BC%8C%E6%96%87%E5%AD%97%E6%8F%9B%E8%A1%8C%EF%BC%8C%E5%BC%B7%E8%BF%AB%E4%B8%8D%E6%8F%9B%E8%A1%8C%E3%80%82.html
```
子節點（針對img破版處理）
```
<script>
  window.onload = img_change;
  function img_change() {
    for(i=0;i<$('.image').length;i++){
      if($('.image')[i].children[0].clientWidth>=$('.image')[i].clientWidth){
        $('.image')[i].children[0].style.width=$('.image')[i].clientWidth+'px';
      }

    }
  }
</script>
//參照樂瑞的detail.html
```
```
調整文本編輯器內圖片按比例縮放
1.在檔案置底處新增如下js,在所要放置處帶入 dropcap 
2.參考貝若國際中的課程詳情頁course_next
<script>
    function desc() {
        console.log(123);  //檢查是否有執行，確認沒問題拿掉
    var img = $(".dropcap").find("p").find("img");  //在dropcap 的下面的 p 標籤 的img 內 中

    for (var i = 0; i < img.length; i++) {
        // $(img[i]).css({"width": "auto", "height": "auto", "max-width" : "100%"});
        $(img[i]).css({
            "height": "auto",
            "max-width": "100%"
        });

        let newNode = document.createElement("p");
        img[i].parentNode.insertBefore(newNode, img[i]);
        }
    };
    window.onload = function()
    {
        desc(); 
    }
</script>
```

