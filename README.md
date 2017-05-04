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

## pageId
Default setting - false. This pulls attached images from current page or post.

## size
Default setting - `thumbnail`. You can either use the standard WP keyword image sizes, or ones you've created all by your onesie using `add_image_size`. You can read about that over here - [https://developer.wordpress.org/reference/functions/add_image_size/]

## single
Default setting - `false`. This determines whether or not you only want the FIRST attached image.

## prepend
Default setting - `<figure>`. The opening tag for your precious image.
	
## append
Default setting - `</figure>`. The closing tag that wraps your precious image.

## orderby
Default setting - `date`. What you chose to have your images sorted by. This accepts the same `orderby` values as the native `get_children`.
