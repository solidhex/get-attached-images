# get-attached-images
WordPress Images Plug-in to pull attached images from post or page.

# Options
`
$defaults = array(
		'pageID' => false,
		'size' => 'thumbnail',
		'single' => false,
		'prepend' => '<figure>',
		'append' => '</figure>',
		'orderby' => 'date',
		'order' => 'DESC',
		'echo' => true
);
`

## pageID
Default setting - `false`. This pulls attached images from current page or post. Alernatively, you can pass in a specific pageID to pull the attached images from that page anywhere you wish.

## size
Default setting - `thumbnail`. You can either use the standard WP keyword image sizes, or ones you've created all by your onesie using `add_image_size`. You can read about that over here - [https://developer.wordpress.org/reference/functions/add_image_size/]

## single
Default setting - `false`. This determines whether or not you only want the FIRST attached image.

## prepend
Default setting - `<figure>`. The opening tag for your precious image.
	
## append
Default setting - `</figure>`. The closing tag for your precious image.

## orderby
Default setting - `date`. What you chose to have your images sorted by. This accepts the same `orderby` values as the native `get_children`.

## order
Default setting - `DESC`. Only two values allowed here, cowboy. `DESC` and `ASC` only, depending on whether you want reverse chronological or vice-versa.

## echo
Default setting - `true`. Whether or not you would like to output the results, or simply return an array of the data.

# Examples
The most basic example would simply be `<?php echo get_attached_images(); ?>` somewhere within your page and post. This plug-in / script need not be within The Loop.

## Adding Parameters
Plug-in should work with either passing in array or a string - e.g. - `<?php echo get_attached_images( array( 'size' => 'large' ) ); ?>` || `<?php echo get_attached_images( 'size=large&pageID=1001' ); ?>`

# Et Cetera
I've mostly set this up for my own personal re-use, but should anyone find it interesting and/or it filled a need for you, let me know. As of right now, if there is a description for the image, it will insert a `figcaption` containing that info. I should probably make this optional, but silence means acceptance.
