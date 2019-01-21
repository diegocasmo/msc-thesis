Description: A summary of the first chapter of the book Recommender Systems by Charu C. Aggarwal
Reference: Aggarwal C.C. (2016) An Introduction to Recommender Systems. In: Recommender Systems. Springer, Cham

### 1.1 An Introduction to Recommender Systems
- "Many receive advice, only the wise profit from it." – Harper Lee
- entity to which the recommendation is provided is referred to as the `user`, and the product being recommended is also referred to as an `item`
- past interests and proclivities are often good indicators of future choices
- collaborative filtering refers to the use of ratings from multiple users in a collective way to predict missing ratings

### 1.2 Goals of Recommender Systems
- the recommendation problem can be formulated as
  - prediction
    - for `m` users and `n` items corresponding to an incomplete `m × n` matrix, use the specified values for training
    - the missing values are to be predicted using a model
  - ranking
    - recommend the top-k items for a particular user
- operational and technical goals of recommender systems
  - relevance: most obvious operational goal of a recommender system is to recommend items that are relevant to the user
  - novelty: recommended an item the user has not seen in the past
  - serendipity: items recommended are somewhat unexpected
  - increasing recommendation diversity: the recommended list contains items of different types (greater chance the user might like at least one of these items)
- presenting meaningful explanations is important to provide the user with an understanding of why they might find a particular item interesting (i.e., why was this item recommended to me?)

### 1.3 Basic Models of Recommender Systems
- collaborative filtering: use user-item interactions as data (ratings, buying behavior)
  - main challenge: the underlaying matrices are sparse
  - most the models focus on leveraging either inter-item correlations or inter-user correlations
  - neighborhood-based collaborative filtering algorithms: ratings of user-item combinations are predicted on the basis of their neighborhoods
    - user-based collaborative filtering: find similar users and recommend items based on them
    - item-based collaborative filtering: find items based on current user 'liked' items and recommend
  - model-based methods: machine learning and data mining methods are used in the context of predictive models
- rating types
  - unbalanced rating scale: when the positive/negative number of rating options is different
  - forced choice rating system: when there is no 'neutral' rating option (the item was either good or bad)
- content-based recommender: use attribute information about the users as data (text profile, keywords)
- there are also hybrid systems, which combine the strengths of various types of recommender systems

### 1.5 Advanced Topics and Applications
- the cold-start problem: the number of initially available ratings might be relatively small
- attack-resistant recommender systems: sellers of products/services have significant economic incentives to manipulate the output of recommender systems. Thus, it's desirable to build systems that can handle such attacks without affecting its overall effectiveness
- group recommender systems: the recommended system is tailored to recommend a particular activity to a group of users rather than a single user
- multi-criteria recommender systems: ratings might be specified on the basis of different criteria by a single user
