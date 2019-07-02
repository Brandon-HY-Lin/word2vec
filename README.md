[tsne_trump_tweets]: https://github.com/Brandon-HY-Lin/word2vec/blob/master/english_twitter/figures/bokeh_plot_trump_tweets.png "t-SNE of Trump's tweets"

# Word2Vec
Analyze Trump's tweets using Word2Vec and display it using t-SNE.

# Methods
  - Word2Vec:
    - Documents are tokenized. Adjacent tokens might be joined as phrases using gensim.models.phrases.Phrase() API.

# Dataset
  - Trump Twitter Archive: Date 2019/01/01 - 2019/05/31
    - Total number of tweets: 2125


# Results
  - 6 keywords and their 10 most similar words are fed into t-SNE.
    - Keyword 1: donald_trump
      - Similar words: throw, suppose, gopleader, jr, shred, clearly, stevehiltonx, jessebwatters, supporters, biggest_scandal
    - Keywords 2: hillary_clinton
      - Similar words: crook, oh, davis, data, democratic_national, wash, acid, russia_investigation, tomfitton_fbi, roger_stone
    - Keywords 3: kim_jong
      - Similar words: economic_powerhouse, summit, nuclear_weapons, chairman_kim, north_korea, dinner, awesome, wise, continuation, hanoi_vietnam
    - Keywords 4: china
      - Similar words: tariff, trade_negotiations, subsidize, asia, renegotiate, best_idea, large_degree, greatly_slow, product_inside, automatically_speed
    - Keywords 5: women
      - Similar words: great_interview, great_men, brave_men, grateful, balance, founder, incredible_men, believer, ways, amy
    - Keywords 6: mexico
      - Similar words: migration, illegals, big_caravan, sadly_murder, strong_immigration, big_contributor, stop_illegals, long_march, americans_die, coyotes
      
      
    ![t-SNE of Trump's tweets][tsne_trump_tweets]
