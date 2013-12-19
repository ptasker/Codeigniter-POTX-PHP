Codeigniter-POTX-PHP
====================

Port of the Drupal Potx project to work with the CodeIgniter language files
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
 
 ```php
 //Sample output
 
$lang['MORE_INFORMATION'] = 'More information';
$lang['SEARCH_FOR_A_SPECIFIC_PROVIDER'] = 'Search for a specific provider';
$lang['NO_RESULTS'] = 'No results';
$lang['CLICK_VIEW_LIST'] = 'View List';
$lang['SEARCH'] = 'Search';
$lang['GREAT_NEWS'] = 'Great news!';
$lang['IS_CURRENTLY_AVAILABLE'] = 'is currently available!';
 
 ```
