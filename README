## jrequire - using java libraries in ruby


This is a thin wrapper for RJB, the Ruby Java Bridge.
It allows you to include Java classes with jrequire and to use them as 
Ruby classes.
It maps the packages and class name to a nested set of Ruby modules. 
The first letter of each module name is capitalized.
For example, java.util.HashMap would become Java::Util::HashMap

### Getting the Source

Performing a git clone on the following repository will get you
the latest source:

    git clone git://github.com/sklemm/jrequire.git 


### Usage

To load the Java lib in your application, do once:

    require 'jrequire'

    libpath = "path/to/your/java/libs"

    classpath = ENV['CLASSPATH'] ||= ''
    classpath += File::PATH_SEPARATOR + File.join(libpath, 'thereswhiskyinthe.jar')

    load_jvm(classpath, ['-Xms128m', '-Xmx1024m'])
    

To use the Java classes in RUby code, do:

    jrequire 'theres.whisky.in.the.Jar'
    
    nice_song = Theres::Whisky::In::The::Jar.new
    

### Licensing and Copyright

Original Work
Copyright (C) 2006 Richard L. Apodaca
Modifications
Copyright (C) 2009 Sebastian Klemm

This file is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License version 2.1 as published by the Free Software
Foundation.

This file is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
Lesser General Public License for more details.


### Support

    klemm.sebi@bluewin.ch
