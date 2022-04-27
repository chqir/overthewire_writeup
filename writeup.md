#over the wire (bandit) challenge writeup list
i am a beginner please do not make fun of me lmao.




#intro
ssh bandit0@bandit.labs.overthewire.org -p 2220
    flag = bandit0

0. nano readme
    flag = boJ9jbbUNNfktd78OOpsqOltutMc3MY1

1. cat ./-
    flag = CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9 

2. nano spaces\ in\ this\ filename
    flag = UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
 
3. cd inhere, ls -A, nano .hidden
    flag = pIwrPrtPN36QITSp3EQaw936yaFoFgAB
 
4. cat -- -file07, p much just catted through all files until i found it :p
    flag = koReBOKuIDDepwhWk7jZC0RTdopnAYKh

5. ls -R(for recursion)A(for all)l(for byte info)
we knew that the file was 1033 bytes, so i just used
this command and searched them manually
    flag = DXjZPULLxYr17uwoI01bNLQbtFemEgo7

6. i knew it had to be owned by bandit7, so
i ran find / -user bandit7, then at the bottom
of the output there was a file '/var/lib/dpkg/info/bandit7.password'
so i just nanod into it and there it was
    flag = HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

7. nano is too op. i used that to enter into
the file then ctrl-w to search it
    flag = cvX2JJa4CFALtqS87jk27qwqGhBM9plV

8. data.txt has a crazy amount of random strings in it,
and i didnt know how i was going to pick out the flag from it.
first it sorts sort data.txt | uniq -c | grep "^ *1 " 
grabs the unique values
then searches for what appears only once
    flag = UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

9.
    flag = 
 
