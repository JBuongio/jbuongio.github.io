---
title: "Joy Buongiorno - Laguna Negra"
layout: piclay
excerpt: "Joy Buongiorno -- Pictures"
permalink: /LN_pictures/
---

# Laguna Negra

#### Photos from the field and under the petrographic microscope:

<ul>
    <?php
        $dirname = "images/LN_pic";
        $images = scandir($dirname);
        shuffle($images);
        $ignore = Array(".", "..");
        foreach($images as $curimg){
            if(!in_array($curimg, $ignore)) {
                echo "<li><a href='".$dirname.$curimg."'><img src='img.php?src=".$dirname.$curimg."&w=300&zc=1' alt='' /></a></li>\n";
            }
        }                 
    ?>
</ul>