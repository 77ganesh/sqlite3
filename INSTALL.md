# Installation to Android device [root required]

First push the compiled binary to sdcard

	adb push /path/to/sqlite3 /sdcard/sqlite3
    
Then copy the binary to system partition and make it executable
	
    adb shell
    su
    mount -o remount,rw /system
    cp /sdcard/sqlite3 /system/xbin/sqlite3
    chmod 4755 /system/xbin/sqlite3
    
Test the sqlite installation by running sqlite3 in adb shell

