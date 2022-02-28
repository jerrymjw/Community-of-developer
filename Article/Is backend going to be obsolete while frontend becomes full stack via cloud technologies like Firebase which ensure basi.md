# Is backend going to be obsolete while frontend becomes full stack via cloud technologies like Firebase which ensure basic server functionality?

[Is backend going to be obsolete while frontend becomes full stack via cloud technologies like Firebase which ensure basic server functionality?](https://www.quora.com/Is-backend-going-to-be-obsolete-while-frontend-becomes-full-stack-via-cloud-technologies-like-Firebase-which-ensure-basic-server-functionality)

Not soon.

But if you’ll allow me to predict the future for a moment…

From an architectural point of view, distinctions between front-end, back-end, and middleware are unpleasantly clunky, and we shouldn’t have to consider them.

Ideally, we should be able to specify every application in terms of data storage, data processing, and (user) interface.

…And nothing more.

In other words, we shouldn’t be thinking about backend and frontend and middleware.

We should only be thinking about — and specifying:

What we want to store, i.e., the database;
How we want to interact with the world outside the system, i.e., the user interface and integrations with other systems; and
What data transformations we want to do in between, i.e., the business logic.
Where that happens — whether on some local server, a cloud-based service, a client device or browser, or somewhere else — should be an optimisation concern that is resolved automatically, invisibly, and possibly dynamically by the system itself.

As a developer, I should not have to specify what runs on the server(s), what runs on the client(s), and what runs in the middleware in between.

That’s an optimisation problem. The system should decide. As a developer, I should only have specify what is required, not where.

Being able to build systems like this is inevitable. It’s just a matter of when.

It’s an unavoidable evolution of systems and application development and associated tools shaped by environmental pressure to deliver more functionality, higher security, and better quality systems at lower cost and shorter timeframes.

The result will be that we will no longer think about backend and frontend and middleware, nor will we use a gaggle of doomed-to-become-obsolete technology like HTML/CSS/JavaScript, SQL, various API specifications and exposed protocols, or languages like PHP, TypeScript/Node.js, Python, Java/JVM and C#/.NET

They’re simply too clunky, too fine-grained, too low-level, too complicated, not expressive enough, and not powerful enough to do the job.

Instead, we’ll use future languages and platforms that will maximise expressiveness; minimise dealing with complex state and exposed machinery like servers, clients, APIs, database and UI languages; and will allow us to focus on specifying executable solutions to business problems without having to know or care where and how our code runs.