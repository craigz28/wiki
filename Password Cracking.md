This will basically be a list of various things tried as part of password cracking research.

Attacking bcrypt hashes

    Cracking the bcrypt hash list appears to be better using CPU rather than GPU when using a small word list (top 8 from 2014)
    Two i7 quad-core CPUs - 8 threads each
    One Windows and one Linux host
    In order to utilize all 8 threads, need an 8 word wordlist, could be more but I want to test the top 8 and be done
    Testing one million hashes at a time on each rig
    Cracking of each one million hash list took around 7 days using above parameters
    Result from the 7 days and top 8 passwords from 2014 are below
    crackcount-day7
    '1234' is at zero most likely indicating that 5 characters is the minimum password length
