# HashDBCreator
This program converts a .txt file to a .HashDB. A hash database is split into pages with each containing x amount of
page entries. Each entry holds a string and its CRCed value accompanied with it. On the reading end, it provides a fast
way to search crced values. The CRC checksum is done on the lower case version of the string, and is the CRC64-ECMA.<br/>

Usage: HashDBCreator.exe "input file path" "output file path" [-v]<br/>


Add the -v option to enable verbose debugging information
