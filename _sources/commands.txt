.. _command-apropos:

Files and directories 
=====================

.. _command-cd:

cd -- Change the current working directory to *directory*.
----------------------------------------------------------

Synopsis
~~~~~~~~

**cd** [options...] [directory]

Description
~~~~~~~~~~~

Change the current working directory to *directory*.

Frequently used options
~~~~~~~~~~~~~~~~~~~~~~~

-p 
    Do not follow symbolic links

-l 
    Do follow symbolic links

Data manipulation
=================

dos2unix -- DOS/Mac to Unix and vice versa text file format converter
---------------------------------------------------------------------

apropos -- search the whatis database for strings
-------------------------------------------------


**apropos** {keywords...}

Description
-----------

apropos searches a set of database files containing short
descriptions of system commands for keywords and displays the
result on the standard output.


----

.. _command-bg:

bg -- background
================

Synopsis
--------

**bg** [jobspec]

Description
-----------

Pleace JOBSPEC in the background, as if it had been started with &.
If JOBSPEC is not present, then the shell's notion of the
*current job* is used, as indicated by the plus sign (+) in output
from the *jobs* command. Using this command on a job that is
stopped will allow it to run in the background.

-----

.. _command-bzip2:

bzip2 -- a block-sorting file compressor
========================================

Synopsis
--------

**bzip2** [option] [filename...]

Description
-----------

bzip2 compresses files using the Burrows-Wheeler block sorting text
compression algorithm, and Huffman coding.

Frequently used options
-----------------------


.. _command-cat:

cat
===

Name
----

cat -- concatenate files and print on the standard output

Synopsis
--------

**cat** [option...] [file...]

Description
-----------

Concatenate FILE(s), or standard input, to standard output.

Frequently used options
-----------------------


.. _command-chmod:

chmod
=====

Name
----

chmod -- change file access permissions

Synopsis
--------

**chmod** [options...] {mode} [files...]

Description
-----------

Change the mode of each FILE to MODE.

Frequently used options
-----------------------

-c, --changes
    like verbose but report only when a change is made

-f, --slient, --quiet
    suppress most error messages

-R, --recursive
    change files and directories recursively

-v, --verbose
    output a diagnostic for every file processed

.. _command-clear:

clear
=====

Name
----

clear -- clear the terminal screen

Synopsis
--------

**clear**

Description
-----------

clear clears your screen if this is possible.

.. _command-cmp:

cmp
===

Name
----

cmp --  compare two files or byte ranges

Synopsis
--------

**cmp** [option...] {-I file1}

Description
-----------

The cmp utility compares two files of any type and writes the
results to the standard output. By default, cmp is silent if the
files are the same; if they differ, the byte and line number at
which the first difference occurred is reported.

Frequently used options
-----------------------


.. _command-comm:

comm
====

Name
----

comm -- Compare two sorted files line by line

Synopsis
--------

**comm** [option...] {left\_file} {right\_file}

Description
-----------

Compare sorted files LEFT\_FILE and RIGHT\_FILE line by line.

Frequently used options
-----------------------

----

.. _command-cp:

cp -- copy files and directories
================================

Synopsis
--------
| cp [OPTION]... [-T] SOURCE DEST
| cp [OPTION]... SOURCE... DIRECTORY
| cp [OPTION]... -t DIRECTORY SOURCE...

Description
-----------

Copy SOURCE to DEST, or multiple SOURCE(s) to DIRECTORY.

Frequently used options
-----------------------

-a, --archive
    same as -dpR

-d 
    same as --no-dereference --preserve=link

-p
    same as --preserve=mode,ownership,timestamps

-r 
    copy recursively, non-directories as files WARNING: use -R instead
    when you might copy special files like FIFOs or /dev/zero

-i, --interactive
    prompt before overwrite

-R, --recursive
    copy directories recursively

----

.. _command-date:

date
====

Name
----

date -- print or set the system date and time

Synopsis
--------

**date** [option...] [+format]

Description
-----------

Display the current time in the given FORMAT, or set the system
date.

Frequently used options
-----------------------

.. _command-df:

df
==

Name
----

df -- report filesystem disk space usage

Synopsis
--------

**df** [option...] [file...]

Description
-----------

df displays the amount of disk space available on the filesystem
containing each file name argument.

Frequently used options
-----------------------

-h, --human-readable 
    print sizes in human readable format (e.g., 1K 234M 2G)


.. _command-diff3:

diff3
=====

Name
----

diff3 -- find differences between three files

Synopsis
--------

**diff3** [option...] {mine} {older} {yours}

Description
-----------

The diff3 command compares three files and outputs descriptions of
their differences.

Frequently used options
-----------------------


.. _command-diff:

diff
====

Name
----

diff -- find differences between two files

Synopsis
--------

**diff** [option...] {from-file} {to-file}

Description
-----------

Concatenate FILE(s), or standard input, to standard output.

Frequently used options
-----------------------



.. _command-dirs:

dirs
====

Name
----

dirs -- Display the list of currently remembered directories.

Synopsis
--------

**dirs** [options...]

Description
-----------

Display the list of currently remembered directories. Directories
are added to the list with the pushd command; the popd command
removes directories from the list.

Frequently used options
-----------------------

- +N 
    Displays the Nth directory (counting from the left of the list
    printed by dirs when invoked without options), starting with zero.

- -N 
    Displays the Nth directory (counting from the right of the list
    printed by dirs when invoked without options), starting with zero.

-c 
    Clears the directory stack by deleting all of the elements.

-l
    Produces a longer listing; the default listing format uses a tilde
    to denote the home directory.

-p 
    Causes dirs to print the directory stack with one entry per line.

-v
    Causes dirs to print the directory stack with one entry per line,
    prefixing each entry with its index in the stack.


.. _command-du:

du
==

Name
----

du --  estimate file space usage

Synopsis
--------

**du** [option...] [file...]

Description
-----------

Summarize disk usage of each FILE, recursively for directories.

Frequently used options
-----------------------

-s, --summarize 
    display only a total for each argument

-h, --human-readable 
    print sizes in human readable format (e.g., 1K 234M 2G)



.. _command-echo:

echo
====

Name
----

echo -- display a line of text

Synopsis
--------

**echo** [options...] [strings...]

Description
-----------

Echo the STRING(s) to standard output.

Frequently used options
-----------------------



.. _command-fg:

fg
==

Name
----

fg -- foreground

Synopsis
--------

**fg** [jobspec]

Description
-----------

This command places the specified job in the foreground, making it
the current job. If JOBSPEC is not present, then the shell's notion
of the current job is used.


.. _command-file:

file
====

Name
----

file --  determine file type

Synopsis
--------

**file** [option...] {file}

Description
-----------

File tests each argument in an attempt to classify it. There are
three sets of tests, performed in this order: filesystem tests,
magic number tests, and language tests. The first test that
succeeds causes the file type to be printed.

Frequently used options
-----------------------



.. _command-find:

find
====

Name
----

find --  search for files in a directory hierarchy

Synopsis
--------

**find** [path...] [expression]

Description
-----------

find searches the directory tree rooted at each given file name by
evaluating the given expression from left to right, according to
the rules of precedence (see section OPERATORS), until the outcome
is known (the left hand side is false for and operations, true for
or), at which point find moves on to the next file name.

Expressions
-----------

The expression is made up of options (which affect overall
operation rather than the processing of a specific file, and always
return true), tests (which return a true or false value), and
actions (which have side effects and return a true or false value),
all separated by operators. -and is assumed where the operator is
omitted. If the expression contains no actions other than -prune,
-print is performed on all files for which the expression is true.

Frequently used options
-----------------------

It is best to place options at the beginning of the expression.

-mindepth levels 
    Do not apply any tests or actions at levels less than levels (a
    non-negative integer).

-maxdepth levels 
    Descend at most levels (a non-negative integer) levels of
    directories below the command line arguments.

-follow 
    Dereference symbolic links. Implies -noleaf.


Frequently used tests
---------------------

Numeric arguments can be specified as:

+n for greater than n

-n for less than n

n for exactly n



-type c 
    File is of type c:

    ::

           b      block (buffered) special

           c      character (unbuffered) special

           d      directory

           p      named pipe (FIFO)

           f      regular file

           l      symbolic link 

-name pattern
    Base of file name (the path with the leading directories removed)
    matches shell pattern pattern.

-atime n
    File was last accessed n\*24 hours ago.

-amin n
    File was last accessed n minutes ago.

-anewer file
    File was last accessed more recently than file was modified.

-ctime n
    File's status was last changed n\*24 hours ago.

-cmin n
    File's status was last changed n minutes ago.


Frequently used actions
-----------------------

-print
    print the full file name on the standard output, followed by a
    newline.

-ls
    list current file in \`ls -dils' format on standard output.

-exec command
    Execute command; true if 0 status is returned. All following
    arguments to find are taken to be arguments to the command until an
    argument consisting of \`;' is encountered.

-ok command
    Like -exec but ask the user first

.. _command-free:

free
====

Name
----

free --  Display amount of free and used memory in the system

Synopsis
--------

**free** [option]

Description
-----------

free displays the total amount of free and used physical and swap
memory in the system, as well as the shared memory and buffers used
by the kernel.

Frequently used options
-----------------------

-s 
    activates continuous polling delay seconds apart.


.. _command-ftp:

ftp
===

Name
----

ftp -- ARPANET file transfer program

Synopsis
--------

**ftp** [option]

Description
-----------

FTP is the user interface to the ARPANET standard File Transfer
Protocol. The program allows a user to transfer files to and from a
remote network site.

Frequently used options
-----------------------

-i 
    Turns off interactive prompting during multiple file transfers.


Frequently used commands
------------------------

The client host with which ftp is to communicate may be specified
on the command line. If this is done, ftp will immediately
attempt to establish a connection to an FTP server on that host;
otherwise, ftp will enter its command interpreter and await
instructions from the user. When ftp is awaiting commands from
the user the prompt \`\`ftp>'' is provided to the user. The
following commands are recognized by ftp:

-cd REMOTE-DIRECTORY 
    Change the working directory on the remote machine to
    REMOTE-DIRECTORY.

-delete REMOTE-FILE 
    Delete the file REMOTE-FILE on the remote machine.

-get REMOTE-FILE [LOCAL-FILE] 
    Retrieve the file remote-file and store it on the local machine.

-glob 
    Toggle filename expansion for mdelete, mget, and mput.

-hash 
    Toggle hash-sign (\`\`#'') printing for each data block
    transferred. The size of a data block is 1024 bytes.

-ls [REMOTE-DIRECTORY] [LOCAL-FILE]
    Print a listing of the contents of a directory on the remote
    machine.

-mdelete [REMOTE-FILES]
    Delete REMOTE-FILES on the remote machine.

-mget REMOTE-FILES
    Expand the REMOTE-FILES on the remote machine and do a get for each
    file name thus produced.

-mput LOCAL-FILES
    Expand the REMOTE-FILES on the remote machine and do a get for each
    file name thus produced.

-passive
    Toggle passive data transfer mode off.

-prompt
    Toggle interactive prompting.

-put LOCAL-FILE [REMOTE-FILE]
    Store a local file on the remote machine.

-pwd
    Print the name of the current working directory on the remote
    machine.

-quit
    A synonym for bye.


.. _command-grep:

grep
====

Name
----

grep -- print lines matching a pattern

Synopsis
--------

**grep** [options] {pattern} [file...]

Description
-----------

grep searches the named input *file* (or standard input if no files
are named, or the file name - is given) for lines containing a
match to the given *pattern*. By default, grep prints the matching
lines.

Frequently used options
-----------------------

-c NUM, --context=NUM
    Print NUM lines of output context. Places a line containing --
    between contiguous groups of matches.

-h, --no-filename
    Suppress the prefixing of filenames on output when multiple files
    are searched.

-i, --ignore-case 
    Ignore case distinctions in both the *pattern* and the input
    files.

-n, --line-number
    Prefix each line of output with the line number within its input
    file.

-v, --invert-match
    Invert the sense of matching, to select non-matching lines.

.. _command-gunzip:

gunzip
======

Name
----

gunzip --  compress or expand files

Synopsis
--------

**gunzip** [option]

Description
-----------

gunzip takes a list of files on its command line and replaces each
file whose name ends with .gz, -gz, .z, -z, \_z or .Z and which
begins with the correct magic number with an uncompressed file
without the original extension. gunzip can currently decompress
files created by gzip, zip, compress, compress -H or pack.

Frequently used options
-----------------------


.. _command-gzip:

gzip
====

Name
----

gzip --  compress or expand files

Synopsis
--------

**gzip** [option]

Description
-----------

Gzip reduces the size of the named files using Lempel-Ziv coding
(LZ77). Whenever possible, each file is replaced by one with the
extension .gz, while keeping the same ownership modes, access and
modification times.

Frequently used options
-----------------------

-d, --decompress, --uncompress 
    Decompress

-#, --fast, --best 
    Regulate the speed of compression using the specified digit #,
    where -1 or --fast indicates the fastest compression method (less
    compression) and -9 or --best indicates the slowest compression
    method (best compression). The default compression level is -6
    (that is, biased towards high compression at expense of speed).

-c, --stdout, --to-stdout 
    Write output on standard output; keep original files unchanged. If
    there are several input files, the output consists of a sequence of
    independently compressed members. To obtain better compression,
    concatenate all input files before compressing them.



.. _command-head:

head
====

Name
----

head -- output the first part of files

Synopsis
--------

**diff** [option...] [file...]

Description
-----------

Print first 10 lines of each FILE to standard output. With more
than one FILE, precede each with a header giving the file name.
With no FILE, or when FILE is -, read standard input.

Frequently used options
-----------------------

-n, --lines=NUMBER
    print first NUMBER lines instead of first 10


.. _command-history:

history
=======

Name
----

history -- lists the history of entered commands

Synopsis
--------

**history** [options...] [files...]

Description
-----------

display a list of commands entered in the shell

Frequently used options
-----------------------



.. _command-jobs:

jobs
====

Name
----

jobs -- list the active jobs

Synopsis
--------

**jobs** [option...] [jobspec...]

Description
-----------

List the active jobs. If JOBSPECS are included, output is
restricted to information about those jobs.

Frequently used options
-----------------------

-l
    Also list PIDs


.. _command-killall:

killall
=======

Name
----

killall --  kill processes by name

Synopsis
--------

**killall** [option]

Description
-----------

killall sends a signal to all processes running any of the
specified commands. If no signal name is specified, SIGTERM is
sent.

Frequently used options
-----------------------


.. _command-kill:

kill
====

Name
----

kill -- terminate a process

Synopsis
--------

**kill** [option]

Description
-----------

The command kill sends the specified signal to the specified
process or process group. If no signal is specified, the TERM
signal is sent. The TERM signal will kill processes which do not
catch this signal.

Frequently used options
-----------------------




.. _command-less:

less
====

Name
----

less -- opposite of more

Synopsis
--------

**less** [file...]

Description
-----------

Less is a program similar to more, but which allows backward
movement in the file as well as forward movement. Also, less does
not have to read the entire input file before starting, so with
large input files it starts up faster than text editors like vi.

Frequently used options
-----------------------



.. _command-ln:

ln
==

Name
----

ln -- make links between files

Synopsis
--------

**ln** [options...] {target...} [link\_name]

Description
-----------

Create a link to the specified TARGET with optional LINK\_NAME. If
LINK\_NAME is omitted, a link with the same basename as the TARGET
is created in the current directory. When using the second form
with more than one TARGET, the last argument must be a directory;
create links in DIRECTORY to each TARGET. Create hard links by
default, symbolic links with --symbolic. When creating hard links,
each TARGET must exist.

Frequently used options
-----------------------

-i, --interactive
    prompt whether to remove destinations

-f, --force
    remove existing destination files

-s, --symbolic
    make symbolic links instead of hard links


.. _command-ls:

ls
==

Name
----

ls -- list directory contents

Synopsis
--------

**ls** [options...] [files...]

Description
-----------

For each file that is a directory, **ls** lists the contents of the
directory; for each file that is an ordinary file, **ls** repeats
its name and any other information requested.

Frequently used options
-----------------------

-a, --al
    do not hide entries starting with .

-l
    use a long listing format



.. _command-mail:

mail
====

Name
----

mail -- send and receive mail

Synopsis
--------

**mail** [option...] {to-addr...}

Description
-----------

Mail is an intelligent mail processing system, which has a command
syntax reminiscent of ed(1) with lines replaced by messages.

Frequently used options
-----------------------


.. _command-man:

man
===

Name
----

man -- format and display the on-line manual pages

Synopsis
--------

**man** {keyword...} {name}

Description
-----------

man formats and displays the on-line manual pages.

Frequently used options
-----------------------


.. _command-more:

more
====

Name
----

more --  file perusal filter for crt viewing

Synopsis
--------

**more** [file...]

Description
-----------

More is a filter for paging through text one screenful at a time.
This version is especially primitve. Users should realize that less
provides more emulation and extensive enhancements.

Frequently used options
-----------------------



.. _command-mount:

mount
=====

Name
----

mount -- mount a file system

Synopsis
--------

**mount** [dir]

Description
-----------

All files accessible in a Unix system are arranged in one big tree,
the file hierarchy, rooted at /. These files can be spread out over
several devices. The mount command serves to attach the file system
found on some device to the big file tree.

Frequently used options
-----------------------



.. _command-mv:

mv
==

Name
----

mv -- move (rename) files

Synopsis
--------

**mv** [options...] {source} {dest}

Description
-----------

Rename SOURCE to DEST, or move SOURCE(s) to DIRECTORY.

Frequently used options
-----------------------

-f, --force
    do not prompt before overwriting equivalent to --reply=yes

-i, --interactive
    prompt before overwrite equivalent to --reply=query

-v, --verbose
    explain what is being done



.. _command-nohup:

nohup
=====

Name
----

nohup -- Run a command immune to hangups, with output to a non-tty

Synopsis
--------

**nohup** {command} [arg...]

Description
-----------

Run COMMAND, ignoring hangup signals.

Frequently used options
-----------------------



.. _command-paste:

paste
=====

Name
----

paste -- merge lines of files

Synopsis
--------

**paste** [option...] [file...]

Description
-----------

Write lines consisting of the sequentially corresponding lines from
each FILE, separated by TABs, to standard output. With no FILE, or
when FILE is -, read standard input.

Frequently used options
-----------------------

-s, --serial
    paste one file at a time instead of in parallel



.. _command-pine:

pine
====

Name
----

pine -- a Program for Internet News and Email

Synopsis
--------

**pine** [option...] [address]

Description
-----------

Pine is a screen-oriented message-handling tool.

Frequently used options
-----------------------


.. _command-popd:

popd
====

Name
----

popd --  Remove the top entry from the directory stack, and cd to
the new top directory.

Synopsis
--------

**popd** [option...]

Description
-----------

Remove the top entry from the directory stack, and cd to the new
top directory. When no arguments are given, popd removes the top
directory from the stack and performs a cd to the new top
directory.

Frequently used options
-----------------------

- +N 
    Removes the Nth directory (counting from the left of the list
    printed by dirs), starting with zero.

- -N 
    Removes the Nth directory (counting from the right of the list
    printed by dirs), starting with zero.



.. _command-ps:

ps
==

Name
----

ps --  report process status

Synopsis
--------

**ps** [option]

Description
-----------

ps gives a snapshot of the current processes. If you want a
repetitive update of this status, use top.

Frequently used options
-----------------------

-e 
    select all processes

-l 
    long format

-f 
    does full listing



.. _command-pstree:

pstree
======

Name
----

pstree -- display a tree of processes

Synopsis
--------

**pstree** [option]

Description
-----------

ps gives a snapshot of the current processes. If you want a
repetitive update of this status, use top.

Frequently used options
-----------------------

-u 
    Show uid transitions. Whenever the uid of a process differs from
    the uid of its parent, the new uid is shown in parentheses after
    the process name.

-p 
    Show PIDs. PIDs are shown as decimal numbers in parentheses after
    each process name. -p implicitly disables compaction.



.. _command-pushd:

pushd
=====

Name
----

pushd -- Save the current directory on the top of the directory
stack and then cd to dir.

Synopsis
--------

**pushd** [option...]

Description
-----------

Save the current directory on the top of the directory stack and
then cd to dir. With no arguments, pushd exchanges the top two
directories.

Frequently used options
-----------------------

- +N 
    Brings the Nth directory (counting from the left of the list
    printed by dirs, starting with zero) to the top of the list by
    rotating the stack.

- -N 
    Brings the Nth directory (counting from the right of the list
    printed by dirs, starting with zero) to the top of the list by
    rotating the stack.

-dir 
    Makes the current working directory be the top of the stack, and
    then executes the equivalent of \`cd dir'. cds to dir.


.. _command-pwd:

pwd
===

Name
----

pwd -- print name of current/working directory

Synopsis
--------

**pwd** [option]

Description
-----------

Print the full filename of the current working directory.

Frequently used options
-----------------------

.. _command-quota:

quota
=====

Name
----

quota -- display disk usage and limits

Synopsis
--------

**quota** [option]

Description
-----------

Quota displays users' disk usage and limits. By default only the
user quotas are printed.

Frequently used options
-----------------------

-s 
    flag will make quota(1) try to choose units for showing limits,
    used space and used inodes.



.. _command-rmdir:

rmdir
=====

Name
----

rmdir -- remove empty directories

Synopsis
--------

**rmdir** [options...] {directory...}

Description
-----------

Remove the DIRECTORY(ies), if they are empty.

Frequently used options
-----------------------

-p, --parents
    remove DIRECTORY, then try to remove each directory component of
    that path name. E.g., \`rmdir -p a/b/c' is similar to \`rmdir a/b/c
    a/b a'.



.. _command-rm:

rm
==

Name
----

rm -- remove files or directories

Synopsis
--------

**rm** [options...] {file...}

Description
-----------

rm removes each specified file. By default, it does not remove
directories.

Frequently used options
-----------------------

-f, --force
    ignore nonexistent files, never prompt

-i, --interactive
    prompt before any removal

-r, -R , --recursive
    remove the contents of directories recursively



.. _command-scp:

scp
===

Name
----

scp -- secure copy

Synopsis
--------

**scp** [option]

Description
-----------

scp copies files between hosts on a network. It uses ssh(1) for
data transfer, and uses the same authentication and provides the
same security as ssh(1).

Frequently used options
-----------------------

-r 
    Recursively copy entire directories.



.. _command-sdiff:

sdiff
=====

Name
----

sdiff -- find differences between two files and merge interactively

Synopsis
--------

**sdiff** {-o} {outfile} [option...] {from-file} {to-file}

Description
-----------

The sdiff command merges two files and interactively outputs the
results to outfile.

Frequently used options
-----------------------


.. _command-sftp:

sftp
====

Name
----

sftp -- Secure file transfer program

Synopsis
--------

**sftp** [option]

Description
-----------

sftp is an interactive file transfer program, similar to ftp(1),
which performs all operations over an encrypted ssh(1) transport.

Frequently used options
-----------------------



.. _command-sleep:

sleep
=====

Name
----

sleep -- delay for a specified amount of time

Synopsis
--------

**sleep** {number} [suffix...]

Description
-----------

Pause for NUMBER seconds. SUFFIX may be \`s' for seconds (the
default), \`m' for minutes, \`h' for hours or \`d' for days.

Frequently used options
-----------------------

.. _command-sort:

sort
====

Name
----

sort -- sort lines of text files.

Synopsis
--------

**sort** [options...] [file...]

Description
-----------

Write sorted concatenation of all FILE(s) to standard output.

Frequently used options
-----------------------



.. _command-split:

split
=====

Name
----

split -- split a file into pieces

Synopsis
--------

**split** [options...] {infile} {outfile}

Description
-----------

Split INFILE into a specified number of line groups, with output
going into a succession of files, OUTFILEaa, OUTFILEab, and so on.
The INFILE remains unchanged. This command is handy if you have a
very long text file that needs to be reduced to a succession of
smaller files. This was often done to email large files in smaller
chunks, because it was at one time considered bad practice to send
single large email messages.

Frequently used options
-----------------------

-n
    Split the INFILE into *n*-line segments. The default is 1000.



.. _command-ssh:

ssh
===

Name
----

ssh -- OpenSSH SSH client

Synopsis
--------

**ssh** [option]

Description
-----------

ssh (SSH client) is a program for logging into a remote machine and
for executing commands on a remote machine. It is intended to
replace rlogin and rsh, and provide secure encrypted communications
between two untrusted hosts over an insecure network.

Frequently used options
-----------------------




.. _command-stat:

stat
====

Name
----

stat -- display file or filesystem status

Synopsis
--------

**stat** [option...] {filename}

Description
-----------

This command displays information about the specified file(s).

Frequently used options
-----------------------



.. _command-sudo:

sudo
====

Name
----

sudo -- execute a command as another user

Synopsis
--------

**sudo** [option...]

Description
-----------

sudo allows a permitted user to execute a command as the superuser
or another user, as specified in the sudoers file.

Frequently used options
-----------------------




.. _command-su:

su
==

Name
----

su -- run a shell with substitute user and group IDs

Synopsis
--------

**su** [option...]

Description
-----------

Change the effective user id and group id to that of USER.

Frequently used options
-----------------------

-, -l, --login 
    make the shell a login shell

-c, --command=COMMAND 
    pass a single COMMAND to the shell with -c

.. _command-tac:

tac
===

Name
----

tac -- concatenate and print files in reverse

Synopsis
--------

**tac** [option...] [file...]

Description
-----------

Write each FILE to standard output, last line first. With no FILE,
or when FILE is -, read standard input.

Frequently used options
-----------------------

-b, --before
    attach the separator before instead of after


.. _command-tail:

tail
====

Name
----

tail -- output the last part of files

Synopsis
--------

**tail** [option...] [file...]

Description
-----------

Print the last 10 lines of each FILE to standard output. With more
than one FILE, precede each with a header giving the file name.
With no FILE, or when FILE is -, read standard input.

Frequently used options
-----------------------

-c, --bytes=N
    output the last N bytes

-f, --follow
    output appended data as the file grows

-n, --lines=N
    output the last N lines, instead of the last 10


.. _command-tar:

tar
===

Name
----

tar -- The GNU version of the tar archiving utility

Synopsis
--------

**tar** [options]

Description
-----------

tar is an archiving program designed to store and extract files
from an archive file known as a tarfile. A tarfile may be made on a
tape drive, however, it is also common to write a tarfile to a
normal file. The first argument to tar must be one of the options:
Acdrtux, followed by any optional functions. The final arguments to
tar are the names of the files or directories which should be
archived.

Frequently used options
-----------------------

-t, --files-from=F
    get names to extract or create from file F

-c, --directory DIR
    change to directory DIR

-x, --exclude-from FILE
    exclude files listed in FILE

-V, --label NAME
    create archive with volume name NAME

-Z, --compress, --uncompress
    filter the archive through compress

-f, --file [hostname:]F
    use archive file or device F (default /dev/rmt0)


.. _command-tee:

tee
===

Name
----

tee -- read from standard input and write to standard output and
files

Synopsis
--------

**tee** [options...] {files}

Description
-----------

Copy standard input to each FILE, and also to standard output.

Frequently used options
-----------------------

-a, --append
    append to the given FILEs, do not overwrite



.. _command-telnet:

telnet
======

Name
----

telnet --  user interface to the TELNET protocol

Synopsis
--------

**telnet** [option]

Description
-----------

The telnet command is used to communicate with another host using
the TELNET protocol.

Frequently used options
-----------------------



.. _command-top:

top
===

Name
----

top -- display top CPU processes

Synopsis
--------

**top** [option]

Description
-----------

top provides an ongoing look at processor activity in real time. It
displays a listing of the most CPU-intensive tasks on the system,
and can provide an interactive interface for manipulating
processes. It can sort the tasks by CPU usage, memory usage and
runtime.

Frequently used interactive commands
------------------------------------

Several single-key commands are recognized while top is running.
Some are disabled if the s option has been given on the command
line.

-h 
    Displays a help screen giving a brief summary of commands, and the
    status of secure and cumulative modes.

-k 
    Kill a process.

-q 
    Quit.

-r 
    Re-nice a process. You will be prompted for the PID of the task,
    and the value to nice it to. Entering a positve value will cause a
    process to be niced to negative values, and lose priority.

-m 
    Toggle display of memory information.

-c 
    Toggle display of command name or full command line.

-p 
    Sort tasks by CPU usage (default).


.. _command-touch:

touch
=====

Name
----

touch -- change file timestamps

Synopsis
--------

**touch** [options...] {file...}

Description
-----------

Update the access and modification times of each FILE to the
current time.

Frequently used options
-----------------------

-a
    change only the access time

-m 
    change only the modification time

-t STAMP
    use [[CC]YY]MMDDhhmm[.ss] instead of current time



.. _command-tr:

tr
==

Name
----

tr -- translate or delete characters

Synopsis
--------

**tr** [options...] {set1} [set2]

Description
-----------

Translate, squeeze, and/or delete characters from standard input,
writing to standard output.

Frequently used options
-----------------------



.. _command-type:

type
====

Name
----

type -- For each *name*, indicate how it would be interpreted if
used as a command name.

Synopsis
--------

**type** [option...] [name...]

Description
-----------

For each name, indicate how it would be interpreted if used as a
command name.

Frequently used options
-----------------------

-t 
    Type prints a single word which is one of \`alias', \`function',
    \`builtin', \`file' or \`keyword', if name is an alias, shell
    function, shell builtin, disk file, or shell reserved word,
    respectively.

-p 
    Type either returns the name of the disk file that would be
    executed, or nothing if \`-t' would not return \`file'.

-a 
    Type returns all of the places that contain an executable named
    file. This includes aliases and functions, if and only if the \`-p'
    option is not also used.


.. _command-umount:

umount
======

Name
----

umount -- umount file systems

Synopsis
--------

**umount** [dir]

Description
-----------

The umount command detaches the file system(s) mentioned from the
file hierarchy.

Frequently used options
-----------------------


.. _command-uniq:

uniq
====

Name
----

uniq --  remove duplicate lines from a sorted file

Synopsis
--------

**uniq** [option...] [input] [output]

Description
-----------

Discard all but one of successive identical lines from INPUT (or
standard input), writing to OUTPUT (or standard output).

Frequently used options
-----------------------


.. _command-watch:

watch
=====

Name
----

watch -- execute a program periodically, showing output fullscreen

Synopsis
--------

**watch** [option] {command}

Description
-----------

watch runs COMMAND repeatedly, displaying its output (the first
screenfull). This allows you to watch the program output change
over time.

Frequently used options
-----------------------


.. _command-wc:

wc
==

Name
----

wc --  print the number of bytes, words, and lines in files

Synopsis
--------

**wc** [option...] [command] [file...]

Description
-----------

Print newline, word, and byte counts for each FILE, and a total
line if more than one FILE is specified.

Frequently used options
-----------------------

-c, --bytes 
    print the byte counts

-l, --lines 
    print the newline counts

-w, --words 
    print the word counts


.. _command-wget:

wget
====

Name
----

wget -- GNU Wget Manual

Synopsis
--------

**wget** [option...] [URL...]

Description
-----------

GNU Wget is a free utility for non-interactive download of files
from the Web. It supports HTTP, HTTPS, and FTP protocols, as well
as retrieval through HTTP proxies.

Frequently used download options
--------------------------------

-nc, --no-clobber 
    If a file is downloaded more than once in the same directory,
    Wget's behavior depends on a few options, including -nc. In certain
    cases, the local file will be clobbered, or overwritten, upon
    repeated download. In other cases it will be preserved.

-c, --continue 
    Continue getting a partially-downloaded file. This is useful when
    you want to finish up a download started by a previous instance of
    Wget, or by another program.


Frequently used directory options
---------------------------------

-nd, --no-directories 
    Do not create a hierarchy of directories when retrieving
    recursively.


Frequently used HTTP options
----------------------------
 
    


Frequently used FTP options
---------------------------

-g on/off, --glob=on/off 
    Turn FTP globbing on or off. Globbing means you may use the
    shell-like special characters (wildcards), like \*, ?, [ and ] to
    retrieve more than one file from the same directory at once.

-passive-ftp 
    Use the passive FTP retrieval scheme, in which the client initiates
    the data connection.

-retr-symlinks 
    When --retr-symlinks is specified, however, symbolic links are
    traversed and the pointed-to files are retrieved.


Frequently used recursive retrieval options
-------------------------------------------

-r, --recursive 
    Turn on recursive retrieving.

-l DEPTH, --level=DEPTH 
    Specify recursion maximum depth level DEPTH.

-k, --convert-links 
    After the download is complete, convert the links in the document
    to make them suitable for local viewing.



.. _command-whatis:

whatis
======

Name
----

whatis -- search the whatis database for complete words.

Synopsis
--------

**whatis** {keyword...}

Description
-----------

whatis searches a set of database files containing short
descriptions of system commands for keywords and displays the
result on the standard output.

Frequently used options
-----------------------



.. _command-whereis:

whereis
=======

Name
----

whereis -- locate the binary, source, and manual page files for a
command

Synopsis
--------

**whereis** [options...]

Description
-----------

whereis locates source/binary and manuals sections for specified
files.

Frequently used options
-----------------------


 
.. _command-which:

which
=====

Name
----

which -- shows the full path of (shell) commands.

Synopsis
--------

**which** [option] {programname}

Description
-----------

For each of its arguments it prints to stdout the full path of the
executables that would have been executed when this argument had
been entered at the shell prompt.

Frequently used options
-----------------------




.. _command-xargs:

xargs
=====

Name
----

xargs --  build and execute command lines from standard input

Synopsis
--------

**xargs** [option...] [command] [initial-argument...]

Description
-----------

Execute COMMAND followed by its optionl INITIAL-ARGUMENTS and
append additional arguments found on standard input. Typically, the
additional arguments are filenames in quantities too large for a
single command line. **xargs** runs COMMAND multiple times to
exhaust all arguments on standard input.

Frequently used options
-----------------------

-n MAXARGS 
    Limit the number of additional arguments to MAXARGS for each
    invocations of COMMAND.

-p 
    Interactive mode. Prompt the user for each execution of COMMAND.



