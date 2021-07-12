# List of Recommender Systems

Recommender systems (or recommendation engines) are useful and interesting pieces of software. I wanted to compare recommender systems to each other but could not find a decent list, so here is the one I created. Please help me keep this post up-to-date by submitting corrections and additions via pull-request, or tweet me [@grahamjenson](https://twitter.com/grahamjenson).

## Software as a Service Recommender Systems

SaaS Recommender systems have many challenges to their development including having to handle multi-tenancy, store and process a massive amount of data and other softer concerns like keeping a clients sensitive data safe on remote servers.

The benefits to using a SaaS recommender system is that you can pay for value with a low overhead rather than having a large upfront investment, they generally have a clear integration path for you to use, and they provide continual development and improvement while you use it.

The SaaS recommender systems are:

1. [Peerius](http://www.peerius.com/) closed, product and e-commerce focused for live and email recommendations. Active and seems very interesting, although little information about the actual product and how it works is available.
1. [Strands](http://recommender.strands.com/) is a closed, product and e-commerce focused system. I think it works by including tracking scripts (a la Google Analytics) on the website, and recommendations widgets. What I really like about Strands is their publishing of case-studies e.g. [Wireless Emporium](http://retail.strands.com/customers/wireless-emporium-case-study/) and white papers like [The Big promise of recommender systems](http://www.aaai.org/ojs/index.php/aimagazine/article/viewFile/2360/2232). Although these do not discuss the exact solutions provided, they give a good overview of their vision and goals of providing recommendations.
1. [SLI Systems Recommender](http://www.sli-systems.com/) A closed recommender system focused on e-commerce, search and mobile.
1. [Using Hadoop on Google Cloud](http://googlecloudplatform.blogspot.co.nz/2014/01/performance-advantages-of-the-new-google-cloud-storage-connector-for-hadoop.html) an example use of Google cloud with benchmarks from recommender system.
1. [ParallelDots](http://www.paralleldots.com/) tool to relate published content
1. [Amazon Machine Learning](http://aws.amazon.com/machine-learning/) machine learning platform to model data and create predictions
1. [Azure ML](http://azure.microsoft.com/en-us/services/machine-learning/) machine learning platform to model data and create predictions
1. [Gravity R&D](http://www.gravityrd.com/) is a company built by some of the winners from the 2009 Netflix prize. They offer a solution that provides targeted, customized recommendations to users of websites. They have some pretty big clients including [DailyMotion](http://www.gravityrd.com/projects#block-views-block-key-partners-key-partners) and a [technology page](http://www.gravityrd.com/technology) which describes their architecture, algorithms, and a list of publications. (suggested by [Marton Vetes](https://www.linkedin.com/in/martonvertes))
1. [Dressipi Style Adviser](https://dressipi.com) is a clothing-specific recommendation service. It incorporates both expert domain knowledge and machine learning to find outfits for occasions or moods.
1. [Sajari](https://www.sajari.com/recommend) is a search, recommendation and matching (e.g. dating website) service. On their site, they also have aggregated a bunch of useful [data-sets](https://www.sajari.com/public-data).
1. [IBM Watson](http://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/) is available through Watson Developer Cloud, which provides REST APIs ([Watson APIs on Bluemix](http://www.ibm.com/cloud-computing/bluemix/watson/)) and SDKs that use cognitive computing to solve complex problems.
1. [Recombee](https://www.recombee.com/) provides REST API, SDKs for multiple languages and graphical user interface for evaluating results. Main features are real time model updates, easy to use query language for filtering and boosting according to complex business rules and advanced features such as options for getting diverse or rotated recommendations. Recombee offers instant account with 100k free recommendation requests per month.
1. [Segmentify](https://www.segmentify.com/) Recommendation Engine, Personalization and Real-Time Analytics tool.
1. [Mr. DLib](http://mr-dlib.org) A recommender-system as-a-service for academic organisations such as digital libraries and reference managers. Mr. DLib provides 'related-article' recommendations, is open-source, and publishes most of it's [data](http://data.mr-dlib.org).

## Open Source Recommender Systems

Most of the non-SaaS recommender systems that are open-source. This may have been because recommender systems are more tailored to clients so not easily made into a product.

The open-source recommender systems are:

1. [The Universal Recommender](https://actionml.com/universal-recommender) Is built on the modern [Correlated Cross-Occurrence Algorithm](http://mahout.apache.org/users/recommender/intro-cooccurrence-spark.html) that uses many indicators of user taste, and so can target most use cases. Source on [github](https://github.com/actionml/harness/blob/develop/docs/ur_simple_usage.md) built-in to the [Harness ML](https://github.com/actionml/harness) server or as a template for the older PredictionIO server ([highest-rated template](http://predictionio.apache.org/gallery/template-gallery/)). Active and commercially supported.
1. [PredictionIO](https://predictionio.apache.org/) is built on technologies [Apache Spark](https://spark.apache.org/), [Apache HBase](http://hbase.apache.org/) and [Spray](http://spray.io/). It is a machine learning server that can be used to create a recommender system. The source can be located on [github](https://github.com/PredictionIO/PredictionIO). Main repository has been *abandoned*.
1. [Raccoon Recommendation Engine](https://www.npmjs.org/package/raccoon) is an open source Node.js based collaborative filter that uses Redis as a store. It is effectively abandoned.
1. [HapiGER](http://www.hapiger.com/) is an open source Node.js collaborative filtering engine, which can use in-memory, [PostgreSQL](http://www.postgresql.org/) or [rethinkdb](http://rethinkdb.com/). Reasonably active development (when I have time :)
1. [EasyRec](http://easyrec.org/) Java and Rest based recommendations. Abandoned
1. [Mahout](http://mahout.apache.org/) Hadoop/linear algebra based data mining
1. [Seldon](http://www.seldon.io) is a Java based prediction engine built on technologies like [Apache Spark](https://spark.apache.org/). It provides a demo movie recommendations application [here](http://www.seldon.io/movie-demo/).
1. [LensKit](http://lenskit.org/) is a Java based research recommender system designed for small-to-medium scale.
1. [Oryx](https://github.com/OryxProject/oryx) [v2](https://github.com/OryxProject/oryx) a large scale architecture for machine learning and prediction (suggested by [Lorand](https://disqus.com/by/disqus_V9tbLHpUxp/))
1. [RecDB](https://github.com/DataSystemsLab/recdb-postgresql) is a PostgreSQL extension to add recommendation algorithms like collaborative filtering directly into the database.
1. [Crab](https://github.com/muricoca/crab) a python recommender based on the popular packages NumPy, SciPy, matplotlib. The main repository seems to be *abandoned*.
1. [predictor](https://github.com/Pathgather/predictor)is a ruby recommender gem. This uses Jaccard or Sorenson-Dice coefficient to priovide both item centric e.g. "Users that read this book also read ..." and user centric e.g. "You read these 10 books, so you might also like to read ..." recommendations. Looks a bit neglected.
1. [Surprise](http://surpriselib.com) A Python scikit for building, and analyzing (collaborative-filtering) recommender systems. Various algorithms are built-in, with a focus on rating prediction.
1. [LightFM](https://github.com/lyst/lightfm) is an actively-developed Python implementation of a number of collaborative- and content-based learning-to-rank recommender algorithms. Using Cython, it easily scales up to very large datasets on multi-core machines and is used in production at a number of companies, including [Lyst](https://www.lyst.com) and [Catalant](https://gocatalant.com/home).
1. [Rexy](https://github.com/kasramvd/Rexy) is an open-source recommendation system based on a general User-Product-Tag concept and a flexible structure that has been designed to be adaptable with variant data-schema. Rexy is written in Python-3.5 in a highly optimized, Pythonic and comprehensive way that makes it so flexible against the changes. It also used Aerospike as the database engine which is a high speed, scalable, and reliable NoSQL database.
1. [QMF](https://github.com/quora/qmf) is a fast and scalable C++ library for implicit-feedback matrix factorization models.
1. [tensorrec](https://github.com/jfkirk/tensorrec) is a TensorFlow recommendation algorithm and framework in Python.
1. [hermes](https://github.com/lab41/hermes) is a recommendation framework for collaborative-filtering and content-based algorithms in PySpark. Main repository has been *abandoned*.
1. [Spotlight](https://github.com/maciejkula/spotlight) utilizes factorization model and sequence model in the back end for building a basic recommendation system. It's a well-implemented Python framework.
1. [Implicit](https://github.com/benfred/implicit) is a Fast Python Collaborative Filtering for Implicit Datasets. This project provides fast Python implementations of several different popular recommendation algorithms for implicit feedback datasets.
1. [recommenderlab](https://cran.r-project.org/web/packages/recommenderlab/index.html) provides a research infrastructure to test and develop recommender algorithms including UBCF, IBCF, FunkSVD and association rule-based algorithms.
4. [CaseRecommender](https://github.com/caserec/CaseRecommender) is a Python implementation of a number of popular recommendation algorithms. The framework aims to provide a rich set of components from which you can construct a customized recommender system from a set of algorithms.
1. [ProbQA](https://github.com/srogatch/ProbQA) is a C++/CUDA recommender system that uses Bayesian approach to learning how answers to its questions map to best recommendations of a target being searched. On GitHub it's available with an example of learning the binary search algorithm. Its application to a [video game recommendation system](http://probqa.com/) is available on the internet as a demo of the engine.
6. [Microsoft Recommenders](https://github.com/Microsoft/Recommenders) contains examples, utilities and best practices for building recommendation systems. Implementations of several state-of-the-art algorithms are provided for self-study and customization in your own applications.
1. [Gorse](https://gorse.io/) is an offline recommender system backend based on collaborative filtering written in Go. It implements mutiple rated or ranked based recommenders and multiple tools ranging from import/export tools to RESTful recommender server.
8. [Nvidia Merlin](https://developer.nvidia.com/blog/announcing-nvidia-merlin-application-framework-for-deep-recommender-systems/) is an end-to-end recommender-on-GPU framework that aims to provide fast feature engineering and high training throughput to enable fast experimentation and production retraining of DL recommender models.

## Non-SaaS Product Recommender Systems

Not very many Non-SaaS Non-OpenSource recommender systems seem to exist. Below is a list:

1. [Dato](http://dato.com/) is a company that provides a python package and servers for business machine learning including many predictive algorithms for recommendations. They also integrate with [Apache Spark](http://blog.dato.com/using-apache-spark-with-graphlab-create) and have great blog posts like **[Why is building custom recommender systems hard? Does it have to be?](http://blog.dato.com/why-is-building-custom-recommender-systems-hard-does-it-have-to-be)**. Their customers include Pandora and StumbleUpon, must be a good product.

## Academic Recommender Systems

Recommender systems are a very active area of research in academia, though few of the generated systems make it out of the lab. Here are a few I have found that did:

1. [Duine Framework](http://sourceforge.net/projects/duine/) a Java based recommendation system that has been abandoned
1. [MyMediaLite](https://github.com/zenogantner/MyMediaLite) C# based in-memory recommender system that has been abandoned
1. **Bonus:** [List of Recommender System Dissertations](http://www.recsyswiki.com/wiki/List_of_recommender_system_dissertations), a useful list to keep up with the current state of recommendations systems in academia
1. [LibRec](http://www.librec.net/) A Java based Recommendations engine with loads of implemented algorithms (suggested by [Saúl Vargas](http://www.dcs.gla.ac.uk/~saul/))
1. [RankSys](https://github.com/RankSys/RankSys) Java Recommendation system for novelty and diversity created by [Saúl Vargas](http://www.dcs.gla.ac.uk/~saul/))
1. [LIBMF](https://www.csie.ntu.edu.tw/~cjlin/libmf/) A Matrix-factorization Library for Recommender Systems
1. [proNet-core](https://github.com/cnclabs/proNet-core) A general-purpose network embedding framework which provides several factorization-based models for recommender systems
1. [Devooght](https://github.com/rdevooght/sequence-based-recommendations) A repository containing collaborative-filtering algorithms based on sequences. 
1. [GRU4Rec](https://github.com/hidasib/GRU4Rec) The original implementation of the algorithm proposed in *Session-based Recommendations with Recurrent Neural Networks* and its follow up in *Recurrent Neural Networks with Top-k Gains for Session-based Recommendations*
1. [Cornac](https://github.com/PreferredAI/cornac) A Python based comparative framework for multimodal recommender systems with a focus on models leveraging auxiliary data (developed by [Preferred.AI](https://preferred.ai/)). 


## Benchmarking Recommender Systems

It is very difficult to benchmark recommender systems, not only because getting good datasets is hard, but different methods and algorithms have different advantages and disadvantages that are difficult to expose.

Here is a list of some benchmarking tools:

1. [TagRec](https://github.com/learning-layers/TagRec) Tag Recommender Benchmarking Framework
1. [RiVaL](http://rival.recommenders.net/) an open source toolkit for recommender system evaluation. Some results are posted [here](http://alans.se/blog/2014/rival/).
1. [Idomaar](http://rf.crowdrec.eu/) is a reference framework for recommender algorithm testing. It is developed in the framework of the [CrowdRec](http://crowdrec.eu) project.

## Media Recommendation Applications

In addition to generic recommender systems, I decided to add a list of applications where recommendations are a core offering, specifically in the domain of media recommendations:

1. [Yeah, Nah](https://github.com/grahamjenson/yeahnah) Movie recommendations app based on [GER](https://github.com/grahamjenson/ger)
1. [Jinni](http://www.jinni.com/) Movie recommendations site
1. [Gyde](http://gyde.tv/) Streaming media recommendations
1. [TasteKid](http://www.tastekid.com/) movies, books, music recommendations. *sent to me by [thelinuxlich](https://github.com/thelinuxlich)*
1. [Gnoosic](http://www.gnoosic.com/) music based on bands. *sent to me by [thelinuxlich](https://github.com/thelinuxlich)*
1. [Pandora](http://www.pandora.com/) music recommendations based on likes and dislikes or songs
1. [Criticker](https://games.criticker.com/ ) Game and movie collaborative recs. *suggested by [ran88dom99](https://github.com/ran88dom99)*
1. [movielens.org](https://movielens.org/) End user movie n book rec by lenskit people. *suggested by [ran88dom99](https://github.com/ran88dom99)*
1. [MAL](https://myanimelist.net/) based [only similar users](http://affinity.animesos.net/)[rec](https://graph.anime.plus/) and [rec](http://www.animerecs.com/)  *suggested by [ran88dom99](https://github.com/ran88dom99)*
1. [NewsPortalUserInteractions](https://www.kaggle.com/gspmoreira/news-portal-user-interactions-by-globocom) A large dataset provided by [globo.com](https://www.globo.com) for news recommendation *suggested by [guedes-joaofelipe](https://github.com/guedes-joaofelipe)*
1. [ContentWise](https://www.contentwise.tv/) UX management solution for digital media entertainment. *suggested by [GiovanniPaoloGibilisco](https://github.com/GiovanniPaoloGibilisco)*

## Books

1. [Practical Recommender Systems](https://www.manning.com/books/practical-recommender-systems) by Kim Falk (Manning Publications). [Chapter 1](https://manning-content.s3.amazonaws.com/download/d/fd45240-cdac-4a2a-bf01-392a34242a37/Falk_PRS_MEAP_V12_ch1.pdf)
2. [Recommender Systems Handbook](https://dl.acm.org/citation.cfm?id=1941884) by Ricci, F. et al.

## Best Practices

1. [Recommenders](https://github.com/microsoft/recommenders) examples and best practices for building recommendations systems by *Microsoft*. 
