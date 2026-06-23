 1) A shell is a text-based interface that lets you talk to your computer.
    There are different types of shells-
    
    Types of Shells:

    Bourne Shell (sh): The original Unix shell, developed by Stephen Bourne.
    C Shell (csh): Known for its C-like syntax, popular for interactive use.
    Korn Shell (ksh): Combines features of sh and csh, offering advanced scripting capabilities.
    Bash (Bourne Again SHell): An improved version of sh, with additional features like command history and tab completion. 

2) simple start, check the version
   bash --version

3) most basic stuff
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

4) Best of each basic 
    ls -lahtS

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


    cd
    cd ..: Move up one directory level
    cd ~: Change to the home directory
    cd -: Switch to the previous directory
    cd /: Change to the root directory     
    
    echo
    -n - Don't add a new line at the end
    -e - Allow special characters like \n for new lines
    -E - Don't allow special characters (default)


    Cat       
    cat command is often used with piping to send the content of files to other commands.
    -n - Add numbers to each line
    -b - Add numbers only to lines with text
    -s - Remove extra empty lines
    -v - Show non-printing characters (except for tabs and end of line)
    for joining 2 files and writing the contents to a third file - cat file1.txt file2.txt > filemain.txt
  
    cp 
    copy file or files inside a folder
    best way = cp -r (for recursive inside a folder) -v (verbose so yk what you did) -u (only new files)
    wildcards- as in git ignore allow for multiple files selected by their identificatin such as extension or starting characters 
    cp *.txt /destination/ will copy all text files to the destination folder

    



    
