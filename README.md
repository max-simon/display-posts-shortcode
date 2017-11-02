# Enhanced Display Posts Shortcode #
This repository is a fork of the original [Display Posts Shortcode Project](https://github.com/billerickson/display-posts-shortcode "Original Package"), but implements some extra features.
Therefore, all parameters of the original packages are still working and can be used. This fork implements in addition:

**pagination**
If there are more posts than you allowed by `posts_per_page` parameter, you can turn on pagination. This is a number indicating the id of the shortcode on the page (therefore the number should be unique for each shortcode on your page). If `wp_pagenavi` is installed, it will use it.<br/>
Default: -1 (Off)<br/>
Example: [display-posts pagination="2"]


**structure**

Specify with a string, in which order the components of the preview should appear. `i` = image, `t` = title, `d` = date, `a` = author, `z` = category, `e` = excerpt and `c` = content. Some components have to be activated to appear (`include_date`, `include_excerpt`, `image_size`).

Default: 'itdazec'

Example: [display-posts structure="tda"] shows only the title, the date and the author


**child_class**

Class applied to the inner wrapper tag for responsive webdesign.

Default: ''

Example: [display-posts wrapper="div" wrapper_class="row" child_class="col-md-6 col-lg-4"]


**show_image_descr**

If this is true, the image caption is printed right below the post image.

Default: false

Example: [display-posts image_size="large" show_image_descr="true"]


**break_after**

Adds container with `clear: both` after a given amount of childs.

Default: 0 (off)

Example: [display-posts wrapper="div" wrapper_class="row" child_class="col-md-6" break_after="2"]


**force_read_more**

If this is true, the read_more button appears even if the text is finished.

Default: false

Example: [display-posts force_read_more="true"]


**calendar_icon**

If this is true, a small calendar icon is printed before the date.

Default: false

Example: [display-posts include_date="true" calendar_icon="true"]



I also add a stylesheet with some basic rules. Feel free to change anything :)
