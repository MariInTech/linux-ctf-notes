# Linux CTF Progress

Completed Challenges:

Challenge #1 - Hidden File

Skills: 
- Hidden File Discovery
- Linux file enumeration

Commands Used:
- ls -la
- cat

Summary:
- Learned how hidden files work in Linux.
- Used ls -la to reveal files beginning with a period (.).
- Used cat to display the contents of a hidden file.
- Learned the difference between viewing files and viewing file contents.

Challenge #7 - Encoded Secret

Skills:
- Base64 Recognition
- Data decoding
- Linux pipes

Commands Used:
- cat
- base64 -d
- echo
- |

Summary:
- Identified Base64 encoded data.
- Learned that encoded data is not the same as encrypted data.
- Performed multiple rounds of decoding.
- Learned how to pass output between commands using a pipe (|).

Challenge #15 - Archive Archaeologist

Skills:
- Archive inspection
- Compressed file analysis
- Nested archive extraction

Commands Used:
- ls -l
- file
- tar -tzf
- tar -xzf

Summary:
- Learned how to identify compressed archive files.
- Inspected archive contents before extraction.
- Followed a nested archive structure through multiple layers.
- Learned the difference between listing archive contents and extracting them. 

Challenge #16 - Symbolic Sleuth

Skills:
- Symbolic links
- Filesystem tracing
- Link analysis

Commands Used:
- ls -l
- readlink
- cat

Summary:
- Learned how symbolic links function in Linux.
- Followed a chain of linked files to locate a target file.
- Used readlink to identify where symlinks pointed.
- Learned the difference between a file and a filesystem reference. 

Challenge #2 - Secret File

Skills:
- Filesystem searching
- Search scope awareness
- Linux permissions

Commands Used:
- pwd
- find /home -name "*secret*"
- cat

Summary:
- Learned how to search the filesystem using the find command.
- Learned that search scope matters (. vs /home).
- Encountered Linux permission boundaries while searching directories.
- Located a target file and displayed its contents.

Challenge #3 - The Largest Log

Skills:
- Log Analysis
- File Investigation
- Binary file inspection
- Text searching

Commands Used:
- ls /var/log
- ls -lh /var/log/large_log_file.log
- file /var/log/large_log_file.log
- strings /var/log/large_log_file.log
- strings /var/log/large_log_file.log | grep "CTF{"

Summary:
- Learned hot to enumerate files within the Linux log directory.
- Identified an unusually large log file by clicking file sizes.
- Used the file command to determine whether a file was text or binary data.
- Learned that large files should be investigated before opening them directly.
- Used strings to extract human-readable content from a binary file.
- Used grep to search extracted text for a specific pattern.
- Learned how Linux administrators and security analysts safely inspect large files during troubleshooting and investigations.

Key Concepts:
- ls -lh displays human-readable file sizes.
- file identifies the type of data stored in a file.
- Strings extract readable text from binary data.
- Grep searches text for matching patterns.
- Combining commands with pipes (|) allows powerful filtering and analysis.
