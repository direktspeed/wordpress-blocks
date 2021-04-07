use @wordpress/* packages
build with @wordpress/scripts

or

use window.wp-* equal to npm package

then

use asset.php or any php to enq files.

## Rules for general flow
The Template escapes the content of wp-post so we can only bypass that via extern enq of files





## Our Flow
We Expose for Admins the ability to Edit/Create new Blocks 

## Rules own flow
- We need a place to store our scripts
- we need a place to offer a api for custom content
- title. post_content, extra filds,



## Integrate into our editor
https://juagonala.com/coding-standards-with-php_codesniffer/

## Cheat Flow 1
enq js with conditional dynamic import that gets access to the file system if your admin.


php example loop inside template 
```php
<table>
<?php 
$myrows = $wpdb->get_results( "SELECT first_name, surname FROM members" );
foreach ( $myrows as $row ) {
echo "<tr><td>" . $row->first_name . "</td><td>" . $row->surname . "</td></tr>";
}
?>
</table>
```
