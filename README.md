    # sedawk-examples
sed awk practical examples

    #remove leading tabs and spaces

vi attendence

    2015-11-08 10:07 16:32pm
    2015-11-09 09:45:30
    spaces in side
			tabs outsid
	tabssd d sf
            spacedsf dsfdsf

    ===solution below == ===

    # cat attendence | sed 's/^[ \t]\+//g'

2015-11-08 10:07 16:32pm
2015-11-09 09:45:30
spaces in side
tabs outsid
tabssd d sf
spacedsf dsfdsf

    Remove multiple tab and spaces 
    cat lists | sed 's/[[:space:]]\+//g'

    cat example.awk
    BEGIN {
	RS="\n\n";
	FS="\n";

    }
    {
	print $1,$2,$3,$4;
    }
    
    awk -f example.awk  filename1

