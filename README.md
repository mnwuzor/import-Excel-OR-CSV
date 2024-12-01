# Import Excel or CSV records into MYSQL using PHP
Learn how to import an excel or CSV records in MySQL using PHP and PhpSpreadsheet Plugin

![image](https://github.com/user-attachments/assets/be7fa9e3-0528-4b59-8d86-51e0f168aca7)

This script will help you import either Excel or CSV records into your applications database. The PHP plugin used in this project is known as PhpSpreadsheet with URL https://phpspreadsheet.readthedocs.io/en/latest/. This plugin makes it very easy to import both Excel or CSV records into your application with less stress.

~~~
<?php session_start(); ?>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>How to Import Excel OR CSV Records into database Using PHP</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    
    <div class="container">
        <div class="row">
            <div class="col-md-12 mt-4">

                <?php
                if(isset($_SESSION['message']))

                {
                    echo "<h4>".$_SESSION['message']."</h4>";
                    unset($_SESSION['message']);
                }
                ?>

                <div class="card">
                    <div class="card-header">
                        <h4>How to Import Excel OR CSV Records into database Using PHP</h4>
                    </div>
                    <div class="card-body">

                        <form action="code.php" method="POST" enctype="multipart/form-data">

                            <input type="file" name="import_file" class="form-control" />
                            <button type="submit" name="save_excel_data" class="btn btn-primary mt-3">Import</button>

                        </form>

                    </div>

                </div>
            </div>
        </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
~~~
Watch the YouTube video on how to setup the script. 

Credit to Funda of Web IT (https://www.fundaofwebit.com/php/import-excel-file-into-mysql-database-in-php#google_vignette) from whose site I saw this plugin and the code he write.
