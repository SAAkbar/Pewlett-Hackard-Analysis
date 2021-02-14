# Pewlett-Hackard-Analysis

## Purpose

The purpose of this assignment was to help Pewlett Hackard with their retirement issue that is about to surface. The first part was to identify the number of retiring employees and their current position. To do this we had to make a dataset of all the employees born between 1952-1955 (those who are about to retire) and then another dataset which gets their most recent position and then finally count the total number of employees from each position to see how much of those positions need to be filled soon. The second part was see which employees are eligible for the mentorship program that will be implemented. To do this we had to create a dataset that contained the names, position and other info of those born in 1965 to see who can then participate in the mentorship program. 

## Results

•	Retirement_titles shows the employee number, first and last name, their title and the time period they had this title for employees born between 1952 and 1955, unfortunately it shows all the titles an employee has had and not just the current title, which is irrelevant to us for this purpose. (Preview seen below) This can been seen in the results as employee 10004 Christian Koblick is seen twice, but you can see that they were first an Engineer and in 1995 they became a Senior Engineer.

![image](https://user-images.githubusercontent.com/76131315/107858893-8c6fe500-6e04-11eb-992a-5b36948d886f.png)

•	Unique_titles corrects the issue of retirement_titles and has all the same information but just the current titles and their time period. (Preview seen below) In the results now, employee 10004 Christian Koblick is only seen once as a a Senior Engineer as that is their current job.

![image](https://user-images.githubusercontent.com/76131315/107858951-b1fcee80-6e04-11eb-89e2-7714edc7cbaf.png)

•	Retiring_titles counts the number of employees for each title in unique_titles which shows how many people in each position is likely going to retire soon. (Table seen below) This shows us that Senior Engineer and Senior Staff have the most people retiring in those positions while on the other side of the spectrum only 2 managers are retiring.

![image](https://user-images.githubusercontent.com/76131315/107858986-d953bb80-6e04-11eb-825a-7c513528b9c8.png)

•	Mentorship_eligibility shows the employee number, first and last name, date of birth, their current title and the time period they had this title for, for employees born in 1965. (Preview seen below) This shows those who are born in 1965 and what positions they are in, this helps because we know that they will likely retire in around 10 years so they can help mentor others. Take employee 10095 Hilari Morton,  


## Summary

By opening up the unique_titles csv we can see that 90398 people will be retiring soon, and by looking at the retiring_titles we can see that Pewlett Hackard will need to replace 90398 people with 2 new Managers, 1761 new Assistant Engineers, 4502 new Technique Leaders, 12243 new Regular Staff, 14222 new  Engineers, 28254 new Senior Staff, and new 29414 Senior Engineers. 

90398 is a lot of positions to fill but before we can do that we need to make sure that we have enough mentors in each position to help so we would run to following code to get the table below

![image](https://user-images.githubusercontent.com/76131315/107859114-554e0380-6e05-11eb-9c3f-a877e722ff62.png)

According to the table above it looks like we should have enough mentors for each position except for Manager which there are 0 mentors available but fortunately that position has only 2 employees who are likely to retire and to be fair we are only checking mentors born in 1965, we can look for the next senior manager to help mentor 2 potential employees to fill those spots. While there should be enough if we look at the numbers we can see that each Senior Staff mentor will need to have at least 56.17 mentees, each Engineer mentors will need to have 30 mentees, each Regular Staff mentors will need to have 55.40 mentees, each Senior Engineer mentors will need to have 142.79 mentees, each Technique Leader mentors will need to have 58.47 mentees, and each Assistant Engineer mentors will need to have 25.90 mentees. Even the two smallest ratios of 25.90:1 and 30:1 mentee to mentors is too much so I would advise to increase the number of mentors to include more than just those born in 1965 maybe included all who were born in the 1960s. Below is the code to the mentors born in the 1960s as well as the number of new mentors for each position. Looking at this now for every position except Staff and Senior Engineers there are more mentors than mentees and for the those two that are less the ratio is now 1.23 mentees to 1 mentors for Staff and 3.14 mentees to mentors for Senior Engineers which are both much more manageable than before.

![image](https://user-images.githubusercontent.com/76131315/107859139-7a427680-6e05-11eb-8c33-fe9a712a8f8b.png)


