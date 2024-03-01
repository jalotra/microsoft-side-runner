Why ? 
- Want to automate downloading of the latest paper from : arxiv-sanity.com 
- Could be that I have a batch job running on a EC2 somewhere and I want to keep backups of arxiv-sanity in case my object 
store crashes.
- Not the ideal way to solve this problem, but this is 1 way.

Manual Flow looks like this : 
- Open arxiv-sanity in a local web browser. 
- Sort on recency
- Click on the latest paper which open a new paper specific page
- Click on "Download PDF" and then finally save in local storage, usually is "Downloads" for almost everyone.

What ? 
- A simple .side <think json> that selenium-side-runner uses to download the top pdf <sorted on time> locally.

How to run ? 
- Just run `bash run.sh`, runs in debug mode so
	- you can see debug logs 
	- see the DAG it follows.
