# Plumber V8 Builder

## Quick Start

This script currently support install prebuilt V8 from tarball, use command to install the prebuilt tarball:

    ./buildv8 --install-only=http://plumberserver.com/data/plumberv8-prebuild.6.3.0.x64.release.tar.gz --prefix=<v8-install-dir>
    
## Full Build

This is the script that downloads and builds Google V8 Javascrip Engine for Plumber's Javascript servlet.
You should use the script to install the compiled V8 library to your machine before enable the Plumber Javascript servlet.

    ./buildv8 --output=<v8-output-dir> --prefix=<v8-install-dir> --install
    
## Use Plumver V8 Library
    
After the script successfully compiled and installed V8, you can configure the Plumber project with

    -Dbuild_javascript=yes -DPLUMBER_V8_PREFIX=<v8-install-dir>
    
To enable javascript servlet.
