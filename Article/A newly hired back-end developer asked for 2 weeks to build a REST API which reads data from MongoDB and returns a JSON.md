# A newly hired back-end developer asked for 2 weeks to build a REST API which reads data from MongoDB and returns a JSON response. Is that too long?

[A newly hired back-end developer asked for 2 weeks to build a REST API which reads data from MongoDB and returns a JSON response. Is that too long?](https://www.quora.com/A-newly-hired-back-end-developer-asked-for-2-weeks-to-build-a-REST-API-which-reads-data-from-MongoDB-and-returns-a-JSON-response-Is-that-too-long)

I’m going to give full credit to the developer for his or her answer. Any estimate from a software developer of “two weeks” should be a huge red flag. It almost always means one or both of:

There isn’t enough information to be able to give any sort of accurate estimate. The task might take an hour, it might take a month… so split the difference, and you get two weeks.
The scope of the task is too broad. Any task with a scope of two weeks should be broken down into smaller tasks. This allows you to see which task is the biggest (and therefore in the dev’s mind, the riskiest), and more importantly allows you to gauge progress in intervals of days rather than weeks so if something is wrong, you can tell sooner and make needed course corrections.
Devs sometimes forget that non-developers aren’t familiar with developer in-jokes and culture and, some might say, passive-aggressive (but highly effective) strategies for dealing with project managers who don’t have the same expertise, or who would be overwhelmed by or have no interest in the details about why properly developed software takes as long as it does.

In this case, the dance is choreographed to work this way:

You: How long will it take you to build a REST API which reads data from MongoDB and returns a JSON response?

Dev: Um. Two weeks? (Note question mark, meaning “care to dance?”)

You: That seems a little long. Can you break it down into smaller tasks for me?

Dev: Ah, sure. I can do that, but I’ll need a little more detail. Can you find out for me how many records there are in the database, if the query results contain text, and if so is the output to be UTF-8 or something else? Also what programming language will be used, and what is the maximum number of records that will need to come back in a single response? And oh, are there any performance requirements, including how many simultaneous queries does the REST API need to be able to serve? And what restrictions are there, if any, on caching of results?

You: Oh. Ok.

<Time passes>

You: Here is the info you wanted.

Dev: Cool. Ok. This doesn’t look too bad. I can have the basic infrastructure done including the conversion from UTF-8 to UTF-16 in a day or two, which will allow the other development to proceed, but it will probably take a week or so to support, test and debug scaling up meet these performance requirements. And that will require… (list of requirements and dependencies).

In short, when you ask a dev for an estimate and you get “two weeks” that normally means there isn’t enough info to answer, and built into the two weeks are at least a couple of days of figuring out exactly what it is that is supposed to be done, and how… and hopefully enough time to actually accomplish the task, whatever it turns out to be.