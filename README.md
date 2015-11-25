# author_word_cloud
#Purpose: list the top unique words for a given author

#To Run
#python word_freq.py


#To Run in R

library(RColorBrewer)
library(wordcloud)
lewis_carol_words <- read.csv("LewisCarroll__unique_words_output", stringsAsFactors = FALSE)
wordcloud(lewis_carol_words$words, min.freq = 1, random.order = FALSE)



virgil_words <- read.csv("Virgil__unique_words_output", stringsAsFactors = FALSE)
wordcloud(virgil_words$words, min.freq = 5, random.order = FALSE)



doyle_words <- read.csv("ArthurConanDoyle__unique_words_output", stringsAsFactors = FALSE)
wordcloud(doyle_words$words, min.freq = 3, random.order = FALSE)






