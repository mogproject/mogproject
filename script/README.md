# shell script
## bk - copy files with timestamp

#### SYNOPSIS
    bk [ source_file | source_dir ] ...  

#### DESCRIPTION
    Copy files or directories to a name with timestamp in the same directory.

    The destination is 'source_file.YYYYMMDD'.
    If there is a file of that name, it will be 'source_file.YYYYMMDD.N'.

    YYYY    Year with century.
    MM      Numeric month, a number from 01 to 12.
    DD      Day, a number from 01 to 31.
    N       Serial number that begins with 0.

#### EXAMPLE
    These examples are in case today is January 23th, 2012.

    bk file1
        'file1' will be copied to 'file1.20120123'.
        If 'file1.20120123' already exists, it will be copied to 'file1.20120123.0' 
        Furthermore if 'file1.20120123.0' already exists,
        it will be copied to 'file1.20120123.1' and so on.
    bk dir1 dir2
        Whole directory 'dir1' will be copied to 'dir1.20120123',
        and 'dir2' will be copied to 'dir2.20120123'
    bk .
        You can use '.' (current directory) and '..' (parent directory).

#### EXAMPLE
    todo

#### EXIT STATUS
    The following exit values are returnd:  
        0    All files were backed up successfully.  
        >0   An error occured.
