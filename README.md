Codeigniter-POTX-PHP
====================

Port of the Drupal Potx project to work with the Codeigniter language files
https://drupal.org/project/potx

#Usage

 ```php
$path = "/var/www/somedir";
$ite = new RecursiveDirectoryIterator( $path );

foreach ( new RecursiveIteratorIterator( $ite ) as $filename => $cur ) {
    //http://php.net/manual/en/class.splfileinfo.php

    if ( $cur->getExtension () == "php" ) {

        $c = file_get_contents ( $cur->getRealPath () );

       _potx_process_file($cur->getRealPath (), 0, '_output_str');

       }
 }
 ```