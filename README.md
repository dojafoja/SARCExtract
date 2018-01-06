# SARCExtract
A SARC and SZS (YAZ0) Extractor for 3DS, Wii U, and Switch games (and some other Nintendo games).
Uses libyaz0.

## Credits:
* NWPlayer123: Original SARCExtract.
* Stella/AboodXD: Ported to Python 3, added support for little endian SARC files and fixed guessing names.
* Dojafoja: Allow any number of files to be passed in. Also supports wildcard use (*.xyz) and dropping multiple files onto the script.

THIS SCRIPT REQUIRES PYTHON 3

USAGE:

You can pass one or more file paths from the command line and also use wildcards (*.xyz) to specify all files with a given extension. These can be used simultaneously from any source location. Providing just a filename without a path prefix will default to the directory from which this program was run.

Example:

To extract an archive that is in the same location as this script you can just specify a filename like this:
'SARCExtract.py archive.szs'

To extract an archive that is in an external location:
'SARCExtract.py c:\downloads\game\archive.szs'

To extract multiple archives:
'SARCExtract.py archive.szs c:\downloads\game\archive.szs f:\game2\archive.szs'

To extract ALL archives in a folder, you can use a wildcard:
'SARCExtract.py c:\downloads\game\\*.szs'

You can use them simultaneously as well:
'SARCExtract.py archive.szs c:\downloads\game\\*.szs f:\game2\\*.szs f:\game3\archive.szs'

You can also drag and drop any number of archive files onto this script as well. This will not work if there is no drophandler setup for Python files. If you are not able to drop files onto the script then there is no drophandler. All new Python installers come with a drophandler by default so installing a newer release of Python from Python.org will probably solve this issue.



