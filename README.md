# Enhanced Display Posts Shortcode #
This repository is a fork of the original [Display Posts Shortcode Project](https://github.com/billerickson/display-posts-shortcode "Original Package"), but implements some extra features.
Therefore, all parameters of the original packages are still working and can be used. This fork implements in addition:

**pagination**<br/>
If there are more posts than you allowed by `posts_per_page` parameter, you can turn on pagination. This is a number indicating the id of the shortcode on the page (therefore the number should be unique for each shortcode on your page). If `wp_pagenavi` is installed, it will use it.<br/>
Default: -1 (Off)<br/>
Example: [display-posts pagination="2"]

**structure**<br/>
Specify with a string, in which order the components of the preview should appear. `i` = image, `t` = title, `d` = date, `a` = author, `z` = category, `e` = excerpt and `c` = content. Some components have to be activated to appear (`include_date`, `include_excerpt`, `image_size`).<br/>
Default: 'itdazec'<br/>
Example: [display-posts structure="tda"] shows only the title, the date and the author

**child_class**<br/>
Class applied to the inner wrapper tag for responsive webdesign.<br/>
Default: ''<br/>
Example: [display-posts wrapper="div" wrapper_class="row" child_class="col-md-6 col-lg-4"]

**show_image_descr**<br/>
If this is true, the image caption is printed right below the post image.<br/>
Default: false<br/>
Example: [display-posts image_size="large" show_image_descr="true"]

**break_after**<br/>
Adds container with `clear: both` after a given amount of childs.<br/>
Default: 0 (off)<br/>
Example: [display-posts wrapper="div" wrapper_class="row" child_class="col-md-6" break_after="2"]

**force_read_more**<br/>
If this is true, the read_more button appears even if the text is finished.<br/>
Default: false<br/>
Example: [display-posts force_read_more="true"]

**calendar_icon**<br/>
If this is true, a small calendar icon is printed before the date.<br/>
Default: false<br/>
Example: [display-posts include_date="true" calendar_icon="true"]


I also add a **stylesheet** with some basic CSS rules. Feel free to change anything :)
