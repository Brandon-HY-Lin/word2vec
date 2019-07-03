[tsne_trump_tweets]: https://github.com/Brandon-HY-Lin/word2vec/blob/master/english_twitter/figures/bokeh_plot_trump_tweets.png "t-SNE of Trump's tweets"
[tsne_website_104]: https://github.com/Brandon-HY-Lin/word2vec/blob/master/chinese_104/figures/tsne_word2vec_website_104.png "t-SNE of Website 104"

# Word2Vec
Analyze Trump's tweets using Word2Vec and display it using t-SNE.

# Methods
  - Word2Vec:
    - Documents are tokenized. Adjacent tokens might be joined as phrases using gensim.models.phrases.Phrase() API.

# Dataset
  - Trump Twitter Archive: Date 2019/01/01 - 2019/05/31
    - Total number of tweets: 2125


# Results
  - Trump's Tweets
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
      
      
  - Website 104
    - 5 keywords and top-10 similar words are then fed into t-SNE.
      - Keyword 1: machine
        - Similar words: learning, deep, scene, bioinformatics, mining, cmm, 或開, intellengent, minimal, vision
        - Explanation:
          - CMM: Coordinate-measuring machine.
      - Keywords 2: learning
        - Similar machine, deep, onnx, supervised, reinforcement, original, unsupervised, dnn, tx, —
        - Explanation:
          - onnx: ONNX is an open format to represent deep learning models. With ONNX, AI developers can more easily move models between state-of-the-art tools and choose the combination that is best for them.
          - tx: Nvidia Jetson TX2 Module (an Embedded device for deploying deep learning APP)
      - Keywords 3: cnn
        - Similar words: rnn, lstm, rcnn, resnet, bnn, 實作練習, gan, twn, vggnet, yolo
        - Explanation:
          - bnn: Binarized Neural Networks
          - twn: Ternary Weight Networks
      - Keywords 4: svm
        - Similar words: knn, random, forest, multivariable, calculus, boosting, 回歸, natworks, sklearn, 聚類
      - Keywords 5: 深度
        - Similar words: recursive, 計學習, 如統, 推理, 貝葉斯, 神經, 常用, bnn, 熱誠與, 並應用
        
    ![t-SNE of Word2Vec results of website 104][tsne_website_104]


# Key APIs
  - Normalization and Tokenization:
    - gensim.utils.simple_preprocess(doc)
  - Stop Words:
    - gensim.parsing.preprocessing.STOPWORDS
  - Lemmatizer:
    - gensim.stem.WordNetLemmatizer().lemmatize()
  - Phrase (Bigram):
    - gensim.models.phrases.Phrase()
    - gensim.models.phrases.Phraser()
    - gensim.models.phrases.Phraser()[docs]
  - Word2Vec:
    - gensim.models.Word2Vec()
    - gensim.models.Word2Vec().build_vocab()
    - gensim.models.Word2Vec().train()
    - gensim.models.Word2Vec()[docs]
 
