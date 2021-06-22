## Добавление

#### Вывод данных из таблицы в виде таблицы
```
if (strcmp($mode, 'select') == 0){
    $result = $tmp->query('select * from '.$table);
    $fields = array_keys($result->fetch(PDO::FETCH_ASSOC));

    $pdo = new PDO("pgsql:host=$host;dbname=$dbname", $dbuser, $dbpass);
    $stmt = $pdo->query('select * from '.$table);
    echo "<table>";
    echo "<tr>";

    foreach ($fields as $elem) {
        echo "<td>" . $elem . "</td>";
    }
    echo "</tr>";
    while ($row = $stmt->fetch())
    {

        echo "<tr>";
        foreach ($fields as $elem) {
            echo "<td>" . $row[$elem] . "</td>";
        }
        echo "</tr>";
    }
    echo "</table>";
}
```
![image](https://user-images.githubusercontent.com/58090572/122997483-b8076b00-d3b4-11eb-8a77-96c32ca928d1.png)