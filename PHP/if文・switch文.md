### if文
```
$x = 20;  
if($x > 10){   //条件式  
  echo "$xは１０より大きい"；  //条件式が成り立つときのみ処理{}が実行される  
}
```
　
### else
```
$x = 20;
if($x == 30){　　　　　　　　　　　　　　　　　　　　　　　 　
  echo "$xは30です"；  
}else{
  echo "$xは３０ではありません"；　　//処理が実行される
}
```

###　elseif
```
$x = 20;
if($x > 30){　　　　　　　　　　　　　　　　　　　　　　　 　
  echo "$xは30より大きい"；  　//fasleなので実行されない
}elseif($x >=20){
  echo "$xは３０以下２０以上"；　　//trueなので実行される
}else{
  echo "$xは２０より小さい"；　　　　//既に当てはまる条件があったため実行されない
}
```

### 複数条件
```
$x = 20;
if($x > 10 && $x < 30){　　　　　　　　　　　　　　　　　　　　　　　 　
  echo "$xは１０より大きい、かつ３０より小さい"；  
}
if($x > 10 || $x < 30){　　　　　　　　　　　　　　　　　　　　　　　 　
  echo "$xは１０より大きい、または３０より小さい"；  
}
```

### 条件の否定
```
$x = 20;
if(!($x == 30)){　　　　　　　　　　　　　　　　　　　　　　　 　
  echo "$xは30ではない"；  
}
```

### switch文
```
if($coin == 0){
  echo "表"；
}elseif($coin == 1){
  echo "裏"；
}esle{
  echo "エラー"；
}
```
```
if($coin == 0){
 switch($coin){　 //$coinは式じゃない
 case 0:
  echo "表"；
  break;    //caseブロックの最後にbreak命令がないとtrueでも次のcaseブロックまで実行されてしまう
 case 1:
  echo "裏"；
  break;
 default:
  echo "エラー"
  break;
 }
 ```
 
