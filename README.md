# pandas-challenge

## PyCitySchools Analysis
We gathered & analyzed data from 15 local high schools, including student info, school budgets, and math/reading test scores. Open PyCitySchools/PyCitySchools.ipynb to explore!

## Misc
- Since we're dealing with such a large dataset (~40k students), it's wise to make sure there aren't any duplicate rows - so I set it up to throw an error message if there were any. There weren't. (Yay!)
- If you wanted to clean up the data more, you could map 2-decimal formatting to all of the test scores (or simply round them all up).

## Notes & conclusions
- Reading scores are almost always higher than math scores - this aligns with typical educational trends we've seen.
- In the final cell, we see that the average % overall passing for a district school is only 53.7%. Charter schools, however, have a much higher combined passing rate of over 90%. If we look at school_size_df & size_summary: the bigger the school, the more likely the school is to be a district school than a charter one, and the bigger the school, the lower the passing rates. This makes sense -- typically, larger schools mean larger class sizes, which typically means teachers and resources are stretched thin and students receive less one-on-one support. Plus, in my own personal experience attending charter and district schools, charter schools tend to have a stronger emphasis on academics.
- It appears that the lower the spending range per student, the higher (on average) the math/reading passing rates are. (See spending_summary.) On its own, this doesn't make a lot of sense, but with the information above, it leads me to believe that the style of school (charter vs. district) has a greater impact on a student's education than a few extra dollars.