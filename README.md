# get-attached-images
WordPress Images Plug-in to pull attached images from post or page.

# Options
`$defaults = array(
		'pageID' => false,
		'size' => 'thumbnail',
		'single' => false,
		'prepend' => '<figure>',
		'append' => '</figure>',
		'orderby' => 'date',
		'order' => 'DESC',
		'echo' => true
);`

##pageId
Default setting - false. This pulls attached images from current page or post.

##size
You can either use the standard WP keyword image sizes, or ones you've created all by your onesie using `add_image_size` which you can read about over here - [https://developer.wordpress.org/reference/functions/add_image_size/]
