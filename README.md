#Plumber V8 Builder

This is the script that downloads and builds Google V8 Javascrip Engine for Plumber's Javascript servlet.
You should use the script to install the compiled V8 library to your machine before enable the Plumber Javascript servlet.

    ./buildv8 --output=<v8-output-dir> --prefix=<v8-install-dir> --install
    
After the script successfully compiled and installed V8, you can configure the Plumber project with

    -Dbuild_javascript=yes -DPLUMBER_V8_PREFIX=<v8-install-dir>
    
To enable javascript servlet.