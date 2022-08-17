# wrangle_undand2
Project 2 of the Udacity Data Analyst Nano Degree to gather, assess, and clean data then act on it through analysis, visualization and/or modelin

<div style="text-align: justify">
    To wrangle the data, we started off by gathering the different as instructed. We needed all our data sources in dataframes that we could work with, so we:
    <ol>
        <li> read the <b>twitter-archive-enhanced.csv</b> to we_rate_dogs dataframe </li>
        <li> used the request library to read the <b>image predictions data</b>, wrote it to a tsvfile, then loaded it as a df</li>
        <li> read in the <b>tweet-json.txt</b> and extracted all the columns we required </li>
    </ol>
    We assessed the data both visually and
    programmatically. It was not very easy visualizing the data visually because the datasets were large and had many columns.
    We however, managed to find some quality problems when we identified quaity issues such as missing values, improper names, null
    values that were not represented as null values. On assessing the data programmatically, we found more issues and confirmed
    some quality issues that we had seen such as missing values that were not detected. We then listed some quality issues and
    tidiness issues that we fixed as listed on the wrangle_act.ipynb.
</div>

<div style="text-align: justify">
After identifying all the issues, we fixed the issues following the structure that we have been following in
    the classroom videos:
    <ol>
        <li>Define: How to fix the issue</li>
        <li>Code: Write lines of code to fix the issue</li>
        <li>Test: Test if the code fixed the issue </ol>
    </ul>
</div>

Between the Code and Test it was a cycle, because at times we will go test only to realize that the code did not work, so we
    had to do back and forth until the issue was solved.
    Once all the issues where solved we merged the datasets. We used an inner join because: 
   <ol>
    <li>Between the we_rate_dogs dataset and the tweet datasets, the merge will give us only ratings that were tweets
        only.</li>
    <li>Between the merged dataset in 1, We then performed an inner join with the image predictions dataset, so that we can only
        get those dogs that have images</li>
    </ol>
    After merging the dataset, we served it to a csv file, loaded it again and gathered a few insights, based on our interest.
    The dataset is a rating of dogs, we therefore were interested in the dogs that have received the highest ratings, and the
    number of dogs stages that existed in the dataset/
