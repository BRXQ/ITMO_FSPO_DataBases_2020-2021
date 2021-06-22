## Добавление

#### Добавление для таблиц доктор, надзиратель
```
if (strcmp($table, 'overseer')==0 || strcmp($table, 'doctor')==0 ){
    $statement = "insert into ".$table." (name, contacts, dob) values ('$name','$contacts', '$dob')";
    $result = $tmp->query($statement);
}
```
![image](https://user-images.githubusercontent.com/58090572/122997208-6d85ee80-d3b4-11eb-8979-1283a4aa9eef.png)
#### Добавление для таблиц животные
```
if (strcmp($table, 'animals')==0){
    $statement = "insert into animals (type, dob, sex) values ('$type','$dob', '$sex')";
    $result = $tmp->query($statement);
}
```
![image](https://user-images.githubusercontent.com/58090572/122997151-61019600-d3b4-11eb-9b8b-f515539654a5.png)