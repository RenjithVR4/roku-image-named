# roku-image-named
This is Roku BrightScript Code to load images pby using the name of the image or Url Path 

Image Loading can be performed by calling , ImageFromPath or ImageNamed
ImageNamed uses the name of the image u dragged into the the images folder
ImageFromPath takes in the full path of the image location, even a url path

Async Loading returns the object and you can call cancel or reload
Sync Loading will return Bitmap but block UI

    ImageNamed(name, {
    	async : true 'Mustbe Specified
    	args : [ ] or { }
    	height : optional
    	width : optional
    	scaleMode : optional default is 1
    	cache : default is true
    	complete : function(id, bitmap, args)
    		
    	end function
    })
    
    ImageFromPath(path, {
    	async : true 'Mustbe Specified
    	args : [ ] or { }
    	height : optional
    	width : optional
    	scaleMode : default is 1
    	cache : default is true
    	complete : function(id, bitmap, args)
    		
    	end function
    })
