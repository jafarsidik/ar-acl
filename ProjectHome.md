# **Ar-acl** #
## Introduction ##
Ar-acl is Access Control Library for codeigniter. This library works with two methods.
  1. User access control by **role**, e.g:
    * "admin/" is admin page that can be accessed only by admin.
    * "salary/" is employer's salary page that can be edited by hrd dept and accounting dept.
  1. User access control by **Very Private Page (VPP) check**, e.g:
    * "profile/edit/john.r" is a page to edit profile information that can be edited by user who logged on with username "john.r".
## Features ##
  1. Restrict user based on role group.
  1. Restrict user to access, edit or delete other user private page.
## Advantages ##
  1. No database needed. Work faster.
  1. No need to modify controller. This library is autoloaded.
## Set Up ##
  1. Add ar\_acl to the autoload libraries to use it.
```
$autoload['libraries'] = array('ar_acl');
```
  1. Copy folder config and libaries to application folder.
## Demo ##
  * If NOT Using Modular Separation (ME, HMVC, Matchbox, or others)
    1. Copy profile.php and salary.php to your controllers.
    1. Try to access all methods and see the message. e.g. http://localhost/yourbase-url/profile/edit/john; http://localhost/yourbase-url/profile/edit/15; http://localhost/yourbase-url/profile/view/john
  * If USING Modular Separation (ME, HMVC, Matchbox, or others)
    1. Copy test folder to your modules folder.
    1. Try to access all methods and see the message. e.g. http://localhost/yourbase-url/test/profile/edit/john; http://localhost/yourbase-url/test/profile/edit/15; http://localhost/yourbase-url/test/profile/view/john
## Download ##
The download also includes test module for test purpose.
[http://code.google.com/p/ar-acl/downloads/list](http://code.google.com/p/ar-acl/downloads/list)
## Discussion ##
Visit [my codeigniter forum](http://codeigniter.com/forums/viewthread/133999/) to share your thought and questions.



Best Regards,

Ardinoto Wahono