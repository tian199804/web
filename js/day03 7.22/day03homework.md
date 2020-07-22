# 题目

1. ```js
   var val = 'c';
   var str = 'Value is' + (val === 'c') ? 'a':'b';
   console.log(str);
   ```

   结果是什么，为什么？  
括号优先级为20，加法优先级为16，条件运算符优先级为4；所以'Value is c'非空字符串为true，true？'a':'b',结果为a

   

2. 一个物体从1000米高的地方落下，每次弹起的高度是前一次高度的0.6倍，问多少次之后，高度小于1米。
```
  var height=1000;
         var count=0;
         while(height>=1){
             height=height*0.6;
             count++;

         }
             
             console.log(count);


```
3. 物品a 2元，b 5元，c 15元，请问刚好花完100元有多少种情况？
```
 var count=0;
   for(var i=0;i<7;i++){
for(var j=0;j<=20;j++){
for( var k=0;k<=50;k++){
if(2*k+5*j+15*i===100){
console.log("a物品",k);
console.log("b物品",j);
console.log("c物品",i);
count++;
}
}
}
}
console.log(count);
```

4. 求s=a+aa+aaa+aaaa+aaa aa ( 一共5个数字 )的值，其中a为一个数字，如 s = 1 + 11 + 111 + 1111 + 11111 （5个数字）
```
 var a=1;
       var val=0;
       var s=0;
        for(var i=0;i<5;i++){
         val=val*10+a;
          s+=val;
        }

console.log(s);
```

5. 孩子吃糖，第一天你给孩子买了一些糖，孩子每天吃糖的一半多一个，到了第10天的时候，发现只剩下一个糖了，问当初第一天买了多少糖？
 
        10    1  
        9     4  
        8    10  
        7    22  
        6    46  
        5    94  
        4   190  
        3   382  
        2   766  
        1   1534  
   
     ```
     for(var i=0, value=1;i<8;i++){
         value=(value+1)*2;
     }
     console.log(value);
     var i=1, value=1;
     while(i<10){
         value=(value+1)*2;
         i++;
     }
     console.log(value);
 ```


6. 最近抖音有对折纸挑战，在不考虑难度的情况下，一张普通的0.0001米厚度的纸，多少次对折后，可以达到最高峰珠穆拉玛峰的高度8848米？

```
var height=0.0001;
    var count=0;
    while(height<8848){
       height=height*2;
       count++;
     }
     console.log(count);
   
```
7. 

   - 输入一个数字，首先判断是否为质数
   - 如果不是质数，将其分解质因数 如：24 = 2 * 2 * 2 * 3，将分解出的质数打印出来。
```
var a=100;
var count=0;
var str="";
var num=a+'=';
 for(i=1;i<=a;i++){
  if(a%i===0){
        count++;
    }
 }
 if(count===2){
        console.log("是质数")
    }else if(count>2){
        for(j=2;j<=a;j++){
           if(a%j===0 ){
           str+=j+"*";
           a=a/j;
           j=1;
          }
}
console.log(num,str);
    }     
    ```
