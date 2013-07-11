Android-BitmapEx
================

Allow to save the Bitmap of Android as Windows BMP file on Android. 

Reference: http://thiscouldbebetter.wordpress.com/2011/08/16/reading-and-writing-a-bmp-file-using-java/   
The original ImageBMP code failed to be used on android, so I did some minor changes
 * 			1. raw pixels serialization with correct order conversion 
 * 			2. make it workable with Android's existing Bitmap object

****
Sample Usage:   

    BitmapEx bmpEx = new BitmapEx(Bitmap.createBitmap(320, 320, Bitmap.Config.ARGB_8888));  
    bmpEx.saveAsBMP(new FileOutputStream("/sdcard/test.bmp"));  
