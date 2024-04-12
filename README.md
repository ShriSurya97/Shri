# MP3-Tag-Reader-and-Editor-for-ID3-V2.3
Author : Shri Surya V.Ra.
Upload Time : March 2024  
Project Tilte : MP3 Tag Reader and Editor for ID3 V2.3  
Description : An MP3 file contains metadata such as title, artist name, album name, year, genre, etc in the header data. ID3 is the metadata  
              container that holds these data in MP3 files. This code allows the user to view the tag stored in the mp3 file and provides an  
	      option to modify the tag data.   
	      Note : Code works only for mp3 files having ID3 V2.3 version tag data.  
  
Language : C  
Compiler Used : GCC  
  
Usage (To be given via command line)  
To view tag data : ./a.out -v mp3_file_name.mp3  
To edit tag data : ./a.out -e -(option_for_tag) <new_tag_data mp3_file_name.mp3  
Options for tags : 	-t -> to edit song title  
       			-a -> to edit song artist name  
            -A -> to edit album name  
        		-y -> to edit year  
        		-m -> to edit comment  
        		-g -> to edit genre  
To get help : ./a.out --help  


*******************************************************************************************************************************  
                                                         FILE DESCRIPTION  
  
main.c     :     Contains the main function and calls the respective functions to do selected process.  
defns.h    :     Contains the user defined data-types for return type of process and status of a function.  
                 It also contains the declerations of view help and error function.  
view.h     :     Contains the user defined data-types for storing the tag and file details and function  
                 declerations necessary for viewing the tag data.  
view.c     :     Contains the function definitions necessary for viewing the tag data stored in an mp3 file  
modify.h   :     Contains the user defined data-types for storing the tag and file details and function  
                 declerations necessary for editing the tag data.  
modify.c   :     Contains the function definitions necessary for editing the tag data stored in an mp3 file.  
  
Additional Files   
testfile.mp3 :     Sample MP3 file that can be used to check the working of the code  
  
*******************************************************************************************************************************  
