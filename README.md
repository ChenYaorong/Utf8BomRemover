# BomSweeper
Remove BOM(Byte Order Marker) from UTF-8 files. 

Wrote this because I had some legacy source codes of several Android projects in UTF-8 with BOM, but couldn't find any software to do batching BOM removing operations on MAC OS or Windows.

##Usage

bs.py [-h] [--type TYPE] path


&ensp;&ensp;&ensp;&ensp;**path**:         path of the target folder or file


&ensp;&ensp;&ensp;&ensp;**-h, --help**:   show this help message and exit

  
&ensp;&ensp;&ensp;&ensp;**--type TYPE**:  file type， if assign the file type, only this type's file will be converted.

###Examples

Convert all files under a folder:

&ensp;&ensp;&ensp;&ensp;```python bs.py /path/to/the/target/folder```

Convert all java files under a folder:

&ensp;&ensp;&ensp;&ensp;```python bs.py /path/to/the/target/folder --type java```

Convert single file:

&ensp;&ensp;&ensp;&ensp;```python bs.py /path/to/the/target/filename ```

<br><br>
**Note**: Thanks to this answer on stackoverflow: http://stackoverflow.com/a/8898439
