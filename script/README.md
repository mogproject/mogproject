# shell script
## bk - backup files

#### SYNOPSIS
    bk [ source_file | source_dir ] ...  

#### DESCRIPTION
    following rules.

        (1) source_file_name.YYYYMMDD
        (2) _source-file-name_._YYYYMMDD_._hhmmss_    , if the file with a name above already exists
        (3) _source-file-name_._YYYYMMDD_._hhmmss_._N_

#### EXAMPLE
    todo

#### EXIT STATUS
    The following exit values are returnd:  
        0    All files were backed up successfully.  
        >0   An error occured.