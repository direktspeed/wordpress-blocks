# Cheats
This file contains advanced concepts and algorythms

## WP_INCLUDATOR
We need the ability to enq files by url while checking that we are a wordpress user
We can do that with a plugin. 

## WP_FILE_API
We need the ability to create and edit files via url while checking if we are a logged in user that has this ability eg admin

## WP_USER_CONTEXT Switch impassionate user view.
We need the ability to do context switching if needed to view it in diffrent user modes. while checking is admin permission
best would be to do that via a url to be flexible.

## WP API THEME that returns JSON without using the wp-api.

## Allow Client side Rendering to be saved as wp-post.
This can't be done efficent without a lot of tooling to handle shadow dom, css sheat creation and not inlining current computed styles and so on.

## Use Template tag and comment tags for script content
We need to review which methods are the best for script inclusion.


## Use JS For server side rendering
To use JS For server side Rendering you need To 
- Run Nodejs and proxy wp 
- Run Nodejs via php 
- Run Nodejs and spawn php instances and return that result without using proxy
- fetch the result from a diffrent server via php.
- Run JS in the browser and save to wp
