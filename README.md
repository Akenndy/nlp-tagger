# NLP Tagger (aka Smart Blogger)

With social media conversations and number of people participating in the conversations growing exponentially, valuable information and expertise is lost in this information overload. Develop an application to summarize free text (social media conversations like Blogs, Posts and Comments) and come out with the keywords (nouns and adjectives). The key parts to the solution are Summarize: Given a free flowing text (English only) the algorithm should identify the keywords (nouns and adjectives). Synonymize: Tag root words for each of the keywords identified. Personalize: build profiles/personas of associates by tying back the root words identified back to the person making such posts

The actual algorithm and the implementation must be withheld to comply with the agreement with Cognizant Technologies that the core logic cannot be distributed to an external party.

## Introduction
NLP Tagger (aka Smart Blogger), is a blogging application implemented over the One Cognizant Platform to develop an enterprise blogging application to allow users to post blogs/articles and discuss. To connect users, we tag their articles accurately so that similar users can find each other, interact and learn more. This can increase collaboration within the company. We also built an intuitive user interface that engages users using gamification. 

## Algorithm and Design

We tag each article by only using it's own content (as we have no other data point). The lack of a corpus leads us to use a derived version of the tf-idf algorithm where we find correlation between all the words in a document and the frequent words, and then extract important words (algorithm described further in reference-papers/keyword-extraction-from-a-single-document-using-word-co-occurrence-statistical-information.pdf). By automatially tagging articles we prevent key data loss, address ineffective feature extraction in a small dataset. We also make this experience fun and competive through gamification, leaderboards to display popular articles or users and award users points/badges based on their activity (inspired from stack overflow).

## Working of the application

In src/
1. Home.html : The home page / main page
2. WritePost.html : Users can write a post (there are two suggestions WritePost1.html and WritePost2.html)
3. Notifications.html : To notify users about any change or update.
4. Search.html : This page is how the ideal search results look like. The other features in the home page such as suggestions,favorites are built around the same basic look, however the arrangement,colors or subtle features vary to make it easier for the users to differentiate.
5. UserProfile.html : This is how the user profile looks like. It has a variety of data to capture all the essential details.

The project report has the detailed screen shots of the final implementation, you can look at it for further information.

## Runner Up for CIO's Challenge for Students, 2013

After rigorous evaluation, we qualified for the finals of the national competition ‘CIO's Challenge for Students, 2013' and won the second place, to
implement the feature of auto­-tagging, we studied Natural Language Processing (NLP) concepts like feature selection and extraction, stemming and n-­grams in this project. Th team comprises of our Mentor (Vignesh Subramanian), Ankush Dhar, Nidhi Jhunjhunwala, and myself (Meghna Natraj)
