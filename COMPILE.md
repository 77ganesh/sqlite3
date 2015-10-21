# Compiling

Download and install android-ndk

From ndk environment, run
	
    ndk-build NDK_PROJECT_PATH=<path_to_sqlite3_folder>
    
    
Now the binaries will be created in `<path_to_sqlite3_folder>/obj/local/<arch>/sqlite3`
The arch can be x86 or armeabi or anything else supported by the ndk. 
The arch is specified in the file `<path_to_sqlite3_folder>/jni/Appilcation.mk`