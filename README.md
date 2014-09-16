RTFConverter
============
RTFConverter as te name implies is a PHP class to convert an RTF file to plain text. RTF or Rich Text Format has some extra characters that form "control words" to format a string in "rich format". When converting an RTF source to plain text these characters have to be parsed individually and proccessed to generate a copy of the plain visible text.

How to use
==========
Start by including the class file
```PHP
include 'RTFConverter.php';
```

Then initialize the class with the target rtf file
```PHP
$rtf = new RTFConverter('my_file_name.rtf');
```

Now call the convert method
```PHP
$plain_text = $rtf->convertToPlainText();
```


Notes
=====
This is converter is just a simple class and might have some bugs.
Some features or control words cannot be converter with this class.



