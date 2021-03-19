# HashDBCreator
This program converts a .txt file to a .HashDB. A hash database is split into pages with each containing x amount of
page entries. Each entry holds a string and its CRCed value accompanied with it. On the reading end, it provides a fast
way to search crced values. The CRC checksum is done on the lower case version of the string, and is the CRC64-ECMA.<br/>

Usage: HashDBCreator.exe "input file path" "output file path" [-v]<br/>


Add the -v option to enable verbose debugging information<br/>

The input file should look like this:<br/><br/>

NEWPAGE MyNewPage<br/>
SomeEntryValueString<br/>
AnotherString<br/>
oooo i like this string<br/>
NEWPAGE ANOTHERPAGE :D<br/>
here is another one<br/>
this many?<br/>
you can have as many <br/>
entries as you want ;)<br/><br/>

Make sure the first line is a NEWPAGE definiton, otherwise preceding entries will be ignored.
