# Movie recommendation algorithm 

Given a movie rating dataset, where an user can rate a movie from 1 to 10 or N/A if they hadn't watched the movie. The goal is to group users and movies simultaneously so that for each user, we can suggest some good movies that this person has not watched.


Input: 
- A matrix, where: 
	- Each row represents an user
	- Each column represents a movie title 
	- Each cell [i. j] is the rating of user i to movie j
- A minimum number of movies $m_0$
- A minimum threshold $\delta$ for the correlation coefficient 

Output: 
A submatrix of $$n$$ rows ($$n$$ users) and $$m \geq m_0$$ columns ($$m$$ movies) so that $$mxn$$ is maximum while there's no N/A in this submatrix, and pairwise correlation coefficient of all rows are at least $$\delta$$.