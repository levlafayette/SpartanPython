# Parallel and High Performance Python

Python is a very popular programming language that provides an object-orientated approach that is extendable and places readability as a priority. However, its integration into a HPC environment does generate confusion, and its performance is generally somewhat less than optimal. This workshop will explain how Pyhton is implemented in Spartan in terms of versions, core modules, and extensions, and local installations. Further, it will examine some of the main changes that one can make to Python code to improve performance, as well as adapting existing Python serial code to different types of parallelisation with job arrays, multithreading extensions, and message passing extensions.

This workshop is designed for people who have prior experience with HPC (the Spartan Essentials workshop is requisite) and assumes some prior knowledge of Python. Please bring your laptop and a desire to make your Python code improve in performace and parallelisation. You will need an SSH client to access Spartan. If you are using Linux and MacOS there should be one built-in. If you are using MS-Windows an option such as Putty (http://putty.org) is recommended. 



## Git

If you check this repository out be aware that it uses Git submodules to manage the reveal.js dependency. To also checkout reveal.js, you will have to either:

### Fetch it all in one hit
`git clone --recursive https://github.com/levlafayette/SpartanPython`

Or:

### Take it step by step

`git clone https://github.com/levlafayette/SpartanPython`   

`git submodule init`    

`git submodule update`   


To regenerate the slides

The SlideExtractor.jar in the root directory will re-create the slides if needed.

To run it ensure that the java version installed is java 8:

`java -version`

should return something along the lines of java version "1.8.0_65".

If it doesn't then install java 8 from here: `http://www.oracle.com/technetwork/java/javase/overview/java8-2100321.html`

Then in a command prompt in the root directory simply issue:

`java -jar SlideExtractor.jar`

You should see something like the following fly by:

`Working on: ./Lessons/Lesson_1.md`
`Writing to: ./Presentation/Lesson_1.html`
`Writing to: ./Presentation/index.html`

## Folders

The directories that make up this project are as follows:

* Lessons - The lesson(s);
* Planning - The plan used to create the course;
* Resources - Resources for this particular run of the training.

