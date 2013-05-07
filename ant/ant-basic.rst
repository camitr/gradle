Another Neat Tool (Apcache ANT)
===============================


*Introduction*


Its a build tool, and provide special support for java programing language.Its a platform independent and has the instruction in the form of xml. Its use to automate the repeatitive task. This can be compiling the source code,running software test and creating files and documentation for the software development.


-- similar tools 

::
	
	Maven,Gradel 


*Java build process includes*

::

	Compilation of source code into java bytecode
	Creation of the .jar file for the distribution of the code
	Creation of the javadoc documentation 

	
Ant uses build.xml as its default configuration file.


*ANT build is based on three blocks*


::

	Tasks
	Targets
	Extension point


Preparation of project
----------------------
#. Need to seprate source file from the genreated file. So java file will be in src folder. All the generated file will be in the build directory.
#. Build dir is splitted into several subdirectories ``classes`` for compiled file ``jar`` [#]_ for the jar file

#. xml file contain the intial a project tag under that target tags are define.

.. [#] Java archive , is a file contain the class, image, and sound files for a java application into a single file.

*Random points from bbb build.xml*

#. HTML-wrapper= Created after the compilation of the flex application. The wrapper embeds the .swf file in the html page by using the <object>  and <embed> tag.



* errors 


# ``The markup in the document following the root element must be well-formed.``  It comes because project tag is closed in the begning. 

# ``warning: 'includeantruntime' was not set, defaulting to build.sysclasspath=last; set to false for repeatable builds``  Solution to this problem including the tag <javac includeantruntime="false" ..../>
  
