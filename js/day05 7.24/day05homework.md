 计算今日离你出生日期经过了多久，精确到分钟。
 ```
 function time(birthday){
            var starttime=new Date(birthday);
             var endtime=new Date();
          var difftime=endtime.getTime()-starttime.getTime(); 
            var diffday=difftime/ (24 * 60 * 60 * 1000);
             var day=Math.floor(diffday);
             var diffhour=(diffday-day)*24;
             var hour=Math.floor(diffhour);
             var minute=Math.floor((diffhour-hour)*60);
             console.log("相差"+day+"天"+hour+"小时"+minute+"分钟");
         }
         time("1998-04-10 05:00:00");
```





 首字母大写。
 var str = 'abcd123';
  str 也有可能不是字符串
   function main(str){
 }
 main('str');
 main(null)
  ===> 'Abcd123'


```
 function main(str){
     if(typeof str=='string'){
    str1=str.charAt(0).toUpperCase()+str.slice(1);
    console.log(str1);
    }else 
    console.log("不是字符串");
  }
 main('abcd123');
 main(null)
 ```
 







 将_后面的小写字母变大写，并且删除_。
假设
 var str = 'a_bgfgh_h_d';
  最后结果 'aBgfghHD'
```
 function trans(str){
     var a=str.split('_');
    var b=a[0];
     for(var i=1;i<a.length;i++){
        b=b+a[i].slice(0,1).toUpperCase()+a[i].slice(1);
     }
     console.log(b);
 }
 trans('a_bgfgh_h_d');
```






 冒泡排序。
```
     function bubbleSort(array){
    //         if(Array.isArray(array)){
             if(array.length<1){
                return array;
             }
            for(var i=0;i<array.length-1;i++){
                for(var j=0;j<array.length-1-i;j++){
                     if(array[j]<array[j+1]){
                         var temp=array[j];
                       array[j]=array[j+1];
                        array[j+1]=temp;
                     }
                 }
             }
            return array;
           console.log(array);
         }
         }
        var array=[1,5,3,2,7,8];
   console.log(sort(array));
        bubbleSort(array);
    ```