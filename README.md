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
