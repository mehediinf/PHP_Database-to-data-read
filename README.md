# PHP_Database-to-data-read
<p>

  <?php


    $result = mysqli_query(mysqli_connect('Localhost','root','','student'),"SELECT *FROM std_info");

    $count = mysqli_num_rows($result);

    if($count>0){

        while($row = mysqli_fetch_array($result)){
            echo "{$row['id']}";
            echo "<br>";
        }

    }

    

?>
</p>
