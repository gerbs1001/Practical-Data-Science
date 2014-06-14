Practical-Data-Science
======================

Practice and classwork from the NYU Stern Practical Data Science Course 
student_file=open("assignment1.txt","r")

lines = 0
experienceunix4=3
experienceunix3=2
experienceunix2=1
experienceunix1=0
experiencedb5=7
experiencedb4=6
experiencedb3=3
experiencedb2=1
experiencedb1=1
experienceprog5=7
experienceprog4=6
experienceprog3=3
experienceprog2=2
experienceprog1=1

for line in student_file:
	lines=lines + 1
	columns = line.strip().split("\t")
	
	#column 1

	if columns[1] == "I have written simple terminal commands or done some system work on the terminal":
		experienceunix4 = experienceunix4+1

	elif columns[1] == ("I have issued a few commands in a terminal based on given instructions") > 0:
		experienceunix3 =experienceunix3+1

	elif columns[1] == ("I have no experience working in a terminal") > 0:
		experienceunix2=experienceunix2+1

	elif columns[1] == ("I dont even understand the question") > 0:
		experienceunix1=experienceunix1+1

	#column 2

	if columns[2] == "I am a database hacker":
		experiencedb5 = experiencedb5+1

	elif columns[2] == ("I can write very complex queries when needed") > 0:
		experiencedb4 =experiencedb4+1

	elif columns[2] == ("I can write simple queries and issue them to a database") > 0:
		experiencedb3=experiencedb3+1

	elif columns[2] == ("I have issued simple queries to a relational database based on given instruction") > 0:
		experiencedb2=experiencedb2+1

	elif columns[2] == ("I have never directly accessed a database") > 0:
		experiencedb1=experiencedb1+1

	#column 3

	if columns[3] == "I am a hacker or have senior-level programming experience":
		experienceprog5 = experienceprog5+1

	elif columns[3] == ("I can write complex programs, am familiar with programming design patterns, software testing, system design, and algorithms") > 0:
		experienceprog4 =experienceprog4+1

	elif columns[3] == ("I can write simple programs to accomplish tasks I encounter") > 0:
		experienceprog3=experienceprog3+1

	elif columns[3] == ("I have written simple programs, based on instructions or a tutorial") > 0:
		experienceprog2=experienceprog2+1

	elif columns[3] == ("I have never programmed before") > 0:
		experiencerprog1=experienceprog1+1



print experienceunix4
print experienceunix3
print experienceunix2
print experienceunix1


print experiencedb5
print experiencedb4
print experiencedb3
print experiencedb2
print experiencedb1


print experienceprog5
print experienceprog4
print experienceprog3
print experienceprog2
print experienceprog1
