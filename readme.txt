##
##
##        Mod title:  Ajax Chat for FluxBB 1.4
##
##      Mod version:  0.8.3
##  Works on FluxBB:  1.4.*
##     Release date:  2011-02-18
##           Author:  adaur (adaur.underground@gmail.com)
##
##      Description:  This mod allows you to display a shoutbox where you want on your
##					  forum. A real room is also available, see notes.
##
##   Affected files:  index.php
##					  header.php
##
##       Affects DB:  Yes
##
##            Notes:  If you want to add a link to the chat in the navbar,
##					  go to admin_options and add it.
##					  See orignal ajax chat readme.txt and
##					  http://sourceforge.net/projects/ajax-chat/
##					  to get more informations about your chat :-)
##					  If you want to disable or unable the shoutbox for the guests,
##					  set $allow_guests to 0 or 1 in include/ajax_chat.php
##
##       DISCLAIMER:  Please note that "mods" are not officially supported by
##                    FluxBB. Installation of this modification is done at 
##                    your own risk. Backup your forum database and any and
##                    all applicable files before proceeding.
##
##


#
#---------[ 1. UPLOAD ]-------------------------------------------------------
#

Files folder to the root of your forum.

#
#---------[ 2. RUN ]----------------------------------------------------------
#

install_mod.php


#
#---------[ 3. DELETE ]-------------------------------------------------------
#

install_mod.php

#
#---------[ 4. OPEN ]---------------------------------------------------------
#

The file(s) where you want the chat to be displayed, for example

index.php


#
#---------[ 5. FIND ]--------------------------------------------------------
#

require PUN_ROOT.'header.php';


#
#---------[ 6. AFTER, ADD ]--------------------------------------------------
#

require PUN_ROOT.'include/ajax_chat.php';


#
#---------[ 7. FIND (steps 7 and 8 for index.php only) ]------------------------
#

$cat_count = 0;


#
#---------[ 8. REPLACE WITH ]------------------------------------------------
#

$cat_count = 1;

#
#---------[ 9. OPEN ]---------------------------------------------------------
#

header.php


#
#---------[ 10. FIND ]--------------------------------------------------------
#

<link rel="stylesheet" type="text/css" href="style/<?php echo $pun_user['style'].'.css' ?>" />


#
#---------[ 11. AFTER, ADD ]--------------------------------------------------
#

<link rel="stylesheet" type="text/css" href="chat/css/shoutbox.css" />


#
#---------[ 12. SAVE/UPLOAD ]-------------------------------------------------
#