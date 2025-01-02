## Preliminary Notes
- Solution aims to identify set of users for which to place harmful content at bottom of feed, rather than censoring users. 
- Claim that the information is not hidden but rather not easy to reach without explicit search (How is this any different?)
- The method is a preventative immunization technique - not counteractive.
- Assumes that information spreads as Independent Cascade (active or inactive nodes).
	- Could consider the network as voter model where misinformation is actively combatted with "accurate" information. 
- NetShield struggles in computing Eigenvalues necessary for its algorithm in large networks as large networks are sparse. 
- Graph is generated from two-week Twitter stream of tweets where tweets contain any kind of mention/retweet.
	- Graph is directed and interaction is defined as anything in the set of comments, likes or retweets. 
- Performance comparison effectively shows SparseShield dominating NetShield. 
- DAVA also takes a lot more time than SparseShield to compute immunizable nodes and then immunize given nodes. 
- SparseShield will save more nodes than DAVA (successfully immunize) - 35k vs 30k nodes in graph of 47k - however counteractive techniques such as SparseShieldPlus and SparseShieldSeedless will perform far worse, saving ~5k nodes.
- DAVA, in general, seems to perform better on smaller budgets whilst SparseShield performs better on larger budgets. 
- Experiment on preventive vs counteractive techniques shows that SparseShield is dominating in performance - number of nodes saved compared to required immunizations. DAVA is best amongst counteractive algorithms (DAVA, Random, SSPlus, SSSeedless, Degree).

## Future Directions 
- Potentially look at modelling with Voter Model instead of Independent Cascade - consider users supply counter-misinformation, such as "community notes" in Twitter. 
- 