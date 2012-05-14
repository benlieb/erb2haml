# Erb2Haml

Bulk convert ugly old ERB files in your rails app into new sleek HAML.
You may even delete just converted files optionally. 

`~$ ruby erb2haml.rb -h`  
`Usage: erb2haml.rb [options] [path1, path2, ...]`  
`` 
`Exampe path_to/erb2haml.rb -fevg file1 file2` 
`Exampe path_to/erb2haml.rb -fg ` 
`Exampe path_to/erb2haml.rb -g path1 path2 ` 
`` 
`pathN - path to directory, if no paths are present calling pwd is used`  
`    -f, --force                      Force delete source ERB files after being converted`
`    -v, --verbose                    Verbose output`
`    -g, --git_delete                 Assumes you're working in a git repo and performs git rm instead of system rm`
`    -e, --files                      operates on single files instead of whole paths`


NOTE: since script is looking for ERB-files recursively, if you define path(s) all ERB files found by that will be converted.
If you don't mention any path current script's directory will be used.


Author: Alexander Kaupanin <kaupanin@gmail.com>
Mods by: Benjamin Lieb http://pixelearth.net
