# Midterm Rubric (Total Point 100, Extra Credit 20)
Midterm project will be more open-ended than labs. Many factors will make the result different from the template, including
different filtering methods for the word. We just need to make sure the solution goes through key steps in the instructions.

Extra credit is only given to students who **work alone**.

**Note: if there is variable naming issue and the code is wrong only because of that, we only deduct 1 point.**

# PART 1: Accessing Twitter API (optional for individuals) (Extra Credit 6)
## Task 1.1 (Extra Credit 4)
## Task 1.2 (Extra Credit 2)

# PART 2: Working with Twitter (Total Point: 5, Extra Credit 4)
## Task 2.1 (optional for individuals) (Extra Credit 4)
## Task 2.2: loading tweet (0)
## Task 2.3 Find the month of the oldest tweet (5)
### creat a dataframe from loaded tweets (1)
### sort the dataframe using "created_at" column (or convert it to month first) (2)
### obtain the oldest tweet month (2)
### Full point if oldest tweet month is correct. Above is useful for deduction of points. (5)
The template answer (April) is incorrect, as it only sorts w.r.t. the string of month. Students can either sort by string or by the number. 

Acceptable answers are: April (4) and October (10).

# PART 3: Twitter Source Analysis (Total Point: 29)
## Task 3.1: merge 16-17 tweet with 17-18 (3)
### read in 16-17 tweets (1)
### concatenate 16-17 dataframe with 17-18 dataframe vertically (2)
Given template is weird since duplicate tweets didn't seem to be removed. 
Students' solution does not need to go through the assertion.
They have to concatenate the two dataframes **vertically**.

The following steps is one example solution:
- extract the "id", "create_at", "source", "full_text" and "retweet_count" columns
- change 'id" column to integer type. Set "id" column as index
- concatenate the two dataframes. And drop the duplicates (while keeping id as index, and without specifying any subsets) in the result. (won't drop id if done this)

## Task 3.2: reformat dataframe (4)
### create or rename into the four columns (2)
### set index as the tweet id (1)
### sort the dataframe by the id (1)
Does not have to match the template. Check the code if students have gone through the instructions.
If they have already reformatted in Task 3.1, then check there what procedures they have done.

## Task 3.3: remove the html tags. Finding the most common device. (7)
### regular expression (1)
### remove HTML tags (2)
### Full point if HTML tags are removed and ignore the above two rubric. (3=1+2)
### count the number of tweets for each source (2)
### plot the sorted tweets (2)
Check result if it still has HTML tags in source. As long as HTML tags are gone, students don't have to use regular expression.

due to loading issue, the plot might not look exactly the same. In this case, check the code.

No need to sort the tweets.

## Task 3.4: analyze w.r.t. device (5)
### first plot: plot either hour column, or roundhour column by countplot (1)
### second plot: extract dataframe where source has the two specified values (2)
### second plot: extract hour or roundhour column from the extracted dataframe (1)
### second plot: distplot the two extracted columns (1)
Does not have to match the template since the dataframe might already be different.

## Task 3.5: compare device for 2016 (4)
### extract dataframe where source has the two specified values and year is in 2016 (2)
### extract hour or roundhour column from the extracted dataframe (1)
### distplot the two extracted columns (1)

## Task 3.6: question (2)
### first question matches with plot (1)
### second question matches with plot (1)
Trump himself will refer to Android, and his staff will refer to iPhone.

Check if the plot matches with the plot in 3.5.

## Task 3.7: Device Analysis (4)
### extract dataframe where source has the two specified values (2)
### extract the year column (1)
### distplot the two columns (1)

# PART 4: Sentiment Analysis (Total Point: 32)
## Task 4.1: read in lexicon and store as dataframe (4)
### read in lexicon txt file and convert to dataframe (1)
### reformat the dataframe to include polarity and token columns (token column is optional) (2)
### set the index of the dataframe to be token (1)
Notice that the lexicon contains multiple sentiment values for same word. Students can ignore this or perform mean or other methods to reduce the value.


## Task 4.2: convert trump tweet text to lowercase (2)
### convert to lowercase (2)

## Task 4.3: remove punctuation by regex (3)
### replace the punctuation regex found ones by space, and store in no_punc column (3)
students don't have to pass the assertion.
## Task 4.4: tidy format (8)
### split the no_punc text into words (2)
### convert the obtained word into vertically concatenated dataframe using expand=True and stack (other methods are allowed too). (3)
### create tidy format columns and copy corresponding values (2)
### set index of tidy format to be the id (1)
As long as end result is correct, students don't have to follow exactly the solution.

## Task 4.5: polarity of sentence (6)
### merge tidy_format with df_sent (2)
### groupby the index and sum the polarity for each tweet (2)
### add the summed polarity to the trump dataframe. Can use merge or any other methods (2)

## Task 4.6: most positive and most negative tweets (4)
### sort dataframe by sentence polarity, and print most negative tweets (2)
### sort dataframe by sentence polarity, and print most positive tweets (2)
The template outputs contain duplicates, but if students have removed them when creating dataframe, they may get different results.
Both outputs containing duplicates and not containing duplicates are fine.

## Task 4.7: analysis if containing specific words (5)
### select the dataframe where the text contains nyt or fox (2)
### distplot the nyt tweet sentiment and fox tweet sentiment (1)
### answer question: any resonable ones will be accepted (2)



# PART 5: Principal Component Analysis (PCA) and Twitter (Total Point: 25)
## Task 5.1: Cleaning up the Data (14)
### remove stopwords (optional to extend the stopwords by http, https, hillary, etc.) (3)
### lemmatize (3)
### count the number of words (2)
### find the 50 largest count of the word (2)
### find the first 5000 ids, or any 5000 selected tweets (2)
### create the document-frequency matrix where rows correspond to tweets, and columns correspond to number of appearances of each word. (2)
### count the appearance of each word, but not just checking if each word appears in the document. (1)

**Students might shift the document-frequency matrix creation to later tasks. This is fine, and we just need to move the grading to the corresponding part.**

Other custom cleaning can also be done, including removing words which are numeric, and removing too-short words. Since they are not mentioned in the instructions, students are free to implement them.

The result will most likely be different from the templates. Check the code.

## Task 5.2: Find the PCA's (5)
### fit the sklearn PCA on the DF matrix (3)
### print the components, and create the correct component matrix, not transformed data (2)
Students might subtract by mean first, which would be fine.
Check the code for correctness.

## Task 5.3: Examine the PCA (2)
### plot the PCA components using heatmap (2)
Don't need to exactly match the template. As long as the code correctly plots, we will give full points.

## Task 5.4: PCA Compare (4)
### select the first and second row/column from the component, but not the transformed data. (2)
### joint plot the two pca component vectors (2)
Since during recitation I said that the column vectors are principle components, students might use the column vectors.
Either row or column is fine since sklearn is treating each component as row vector.

# PART 6: Twitter Engagement (Total Point: 9)
## Task 6.1: popular retweeted words (7)
### find words that appear in at least 25 tweets (3)
### group by word to compute mean or any statistics (median, sum, etc.) of the retweet count for each word (2)
### sort the retweet count to find the top 20 (2)
The solution may not match the template, and we should check the code.

## Task 6.2: bar plot (2)
### bar plot of the retweet count (2)
The solution may not match the template, and we should check the code.

# PART 7: Conclusion (Optional for Individual) (Extra Point 6)
## Task 7.1 (Extra Credit 3)
## Task 7.2 (Extra Credit 3)

# PART 8: - Analyze Up-to-Date Data (Optional for Individual) (Extra Point 2)

# Find Something interesting (Optional for Individuals) (Extra Point 2)


