### Get filename from any path
os.path.basename(path) : It is used to return the basename of the file i.e file name from the path given. 
  print(os.path.basename("/baz/filename.txt"))
  o/p - filename.txt
  
### Get Directory name from any path
os.path.dirname(path) : It is used to return the directory name from the path given.
  print(os.path.dirname("/baz/foo"))
  o/p - '/baz'
  
### Check directory exists or not
 os.path.isdir(path) : This function specifies whether the path is existing directory or not. 
 print(os.path.isdir("C:\\Users"))
 o/p - True
 
### Convert path according to Python format
os.path.normcase(path) : This function normalizes the case of the pathname specified. In Unix and Mac OS X system it returns the pathname as it is . But in Windows it converts the path to lowercase and forward slashes to backslashes. 
  print(os.path.normcase("/BAz"))
  o/p - '\\baz'
  
### Normalize path as per Python format
os.path.normpath(path) : This function normalizes the path names by collapsing redundant separators and up-level references so that A//B, A/B/, A/./B and A/foo/../B all become A/B. On Windows, it converts forward slashes to backward slashes .
  print(os.path.normpath("foo/./bar"))
  o/p - 'foo\bar'
  
### Get current Directory path
Using os.getcwd() method to get current working directory

### Absolute and Relative path
Absolute path include root directory
"C:\\Users\\sam\projects""
Relative Path
..\\projects

~ocean\\otter
Note - explaination pending

### Get Parent directory
BASE_DIR is pointing to the parent directory of PROJECT_ROOT

**PROJECT_ROOT = os.path.dirname(os.path.abspath(__file__))**
os.path.dirname() function simply removes the last segment of a path.

**BASE_DIR = os.path.dirname(PROJECT_ROOT)**
os.path.abspath() function is used to turn that into an absolute path before removing just the filename and storing the full path to the directory the module lives in in PROJECT_ROOT.


### Needs to explain
path = (os.path.realpath(__file__))

### Path slash change
import os
path = "C:\\temp\myFolder\example\\"
newPath = path.replace(os.sep, '/')
print(newPath)  # -> C:/temp/myFolder/example/

### Os path Join
import os
path = "/home"
print(os.path.join(path, "User/Desktop", "file.txt"))


