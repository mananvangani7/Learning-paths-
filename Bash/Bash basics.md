 # 1) A shell is a text-based interface that lets you talk to your computer.
    There are different types of shells-
    
   ## Types of Shells:

    Bourne Shell (sh): The original Unix shell, developed by Stephen Bourne.

    C Shell (csh): Known for its C-like syntax, popular for interactive use.

    Korn Shell (ksh): Combines features of sh and csh, offering advanced scripting capabilities.

    Bash (Bourne Again SHell): An improved version of sh, with additional features like command history and tab completion. 


# 2) simple start, check the version
   bash --version

 # 3) most basic stuff
    ls - List directory contents

    cd - Change the current directory

    pwd - Print the current working directory

    echo - Display a line of text

    cat - Concatenate and display files

    cp - Copy files and directories

    mv - Move or rename files

    rm - Delete files or folders

    touch - Create an empty file or update its time

    mkdir - Create a new folder


# 4) Best of each basic 
    
   ## ls -lahtS

    -l - Long listing format

    -a - Include hidden files

    -h - Human-readable sizes

    -t - Sort by modification time

    -r - Reverse order while sorting

    -R - List subdirectories recursively

    -S - Sort by file size

    -1 - List one file per line

    -d - List directories themselves, not their contents

    -F - Append indicator (one of */=@|) to entries    


   ##  cd
    cd ..: Move up one directory level

    cd ~: Change to the home directory

    cd -: Switch to the previous directory

    cd /: Change to the root directory     
    
   ## echo
    -n - Don't add a new line at the end

    -e - Allow special characters like \n for new lines

    -E - Don't allow special characters (default)


   ## Cat       
    cat command is often used with piping to send the content of files to other commands.

    -n - Add numbers to each line

    -b - Add numbers only to lines with text

    -s - Remove extra empty lines

    -v - Show non-printing characters (except for tabs and end of line)

    for joining 2 files and writing the contents to a third file - cat file1.txt file2.txt > filemain.txt

  
   ## cp 
    copy file or files inside a folder

    best way = cp -r (for recursive inside a folder) -v (verbose so yk what you did) -u (only new files)

    wildcards- as in git ignore allow for multiple files selected by their identificatin such as extension or starting characters 

    cp *.txt /destination/ will copy all text files to the destination folder


   ## mv 
    used for moving or renaming 

    best use case - move only newer files that are not present in a new folder 

    other use case- 

    -i - Ask before replacing files

    -u - Move only if the source is newer

    -v - Verbose mode, show files being moved

   ## man

    manual for any command

    just by typing man infront of a  command name  

   ## grep
    
    to search for text using a pattern 

    grep 'pattern' file.extension

    finds the pattern and prints the line 

    best flag= add -i to ignore case 

    also can be used with regular expression to find specific things 

 ## awk 
   
   for manipulating data, getting small overviews, pattern scanning. data extraction from text files 

   example of just printing first column that is seperated by ","
   awk -F"," '{print $1}' filename.csv

       rators
       The operators in AWK, in order of decreasing precedence, are:

       (...)       Grouping

       $           Field reference.

       ++ --       Increment and decrement, both prefix and postfix.

       ^           Exponentiation.

       + - !       Unary plus, unary minus, and logical negation.

       * / %       Multiplication, division, and modulus.

       + -         Addition and subtraction.

       space       String concatenation.

       |   |&      Piped I/O for getline, print, and printf.

       < > <= >= == !=
                   The regular relational operators.

       ~ !~        Regular expression match, negated match.

       in          Array membership.

        &&          Logical AND.

       ||          Logical OR.

       ?:          The  C  conditional  expression.   This has the form expr1 ? expr2 : expr3.  If expr1 is true, the
                   value of the expression is expr2, otherwise it is expr3.  Only one of expr2 and  expr3  is  evalu‐
                   ated.

       = += -= *= /= %= ^=
                   Assignment.   Both absolute assignment (var = value) and operator-assignment (the other forms) are
                   supported.

 ## cut command
  Simply extract fields or to see data by passing a delimiter between the text 

  cut -f1 file.txt will show the first column 

  cut -d',' file.txt will show the data with the delimitter of ','

  cut -f1-2 file.txt will show the first columns or fields 

 ## sort 

  -r - Sort in reverse order

  -n - Sort numbers correctly

  -k - Sort by a specific column

  -u - Remove duplicate lines

  -t - Specify a delimiter for fields

  just basically sort lines inside a file on basis of a column or field

  best = sort -t',' -n 

  ( i dont understand how to use column with -k in this at all )

  ## tail 

  to display the last part of a file 

  options/flags 

  -n [number]: Display the last [number] lines of the file.

  -f: Follow the file as it grows, useful for monitoring log files.

  -c [number]: Display the last [number] bytes of the file.

  --pid=[pid]: Terminate after the process with the given PID dies.

  --retry: Keep trying to open a file even if it is inaccessible.

  so best- tail -n 10 -f


  # System Monitoring 

  ## Basics for system 
   
    1) ps - current processes 
           -e - Show all processes
           -f - Show detailed information
           -u - Show processes for a specific user
           -a - Show all processes with a terminal
           -x - Show processes without a terminal 

           so best- ps -ef
    2) top - all tasks of linux and uses real time monitoring 

            so best- top -d 5

    3) df - disk space usage 

            best- df -ah

    4) du - file space usage
            
            best- du -ahsc

    5) free - for checking ram usage 
           
            best- free -hgt

    6) uptime and kill [PID]
   
    7) ping- to check network connection by sending packets 
            eg- ping -q google.com
    
    8)  
   



    



    
