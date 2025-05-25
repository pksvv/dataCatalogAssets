> **Speaker 1:**  
It really feels like we're drowning in data these days, doesn't it?

<div align="right">

> **Speaker 2:**  
Oh, absolutely. There's just so much of it. Everyone talks about potential, but actually grasping the key ideas, figuring out how they all connect. That can be tough.

</div>

> **Speaker 1:**  
Yeah, it's a challenge. So for this deep dive, we thought we'd carve out a clear path for you. We're focusing on a really critical area in modern data thinking,

<div align="right">

> **Speaker 2:**  
Oh, cheers. Understanding data products, specifically within the whole data mesh framework. Write the data mesh context. It's becoming so important. We've gathered some really excellent resources. Think data mesh in action, the data mesh architecture book, focusing on designing these products. Okay. Some great articles from modern data 101 on pipelines and actually building the things. Plus some overviews on, you know, what is a data product? How do you measure if it's any good?

</div>

> **Speaker 1:**  
Sounds comprehensive.

<div align="right">

> **Speaker 2:**  
We're trying to cut through the noise. Really? Think of this as your guide. Hmm. Our mission is to distill that core knowledge, give you a solid grip on data products in a mesh. So what they are, how they get built, how we know if they're working.

</div>

> **Speaker 1:**  
Exactly. We want clarity, actionable insights, you know, without making your head spin with too much technical detail.

<div align="right">

> **Speaker 2:**  
Okay. Let's dive in then. The absolute foundation. What is a data product in simple terms?

</div>

> **Speaker 1:**  
Okay. So the core definition, people use it something like an autonomous and read optimized standardized data unit, containing at least one data set created for satisfying user needs.

<div align="right">

> **Speaker 2:**  
Right. That's quite packed. Let's break it down. Autonomous. Means it stands alone, managed by a specific team, usually a domain team that's not just floating around.

</div>

> **Speaker 1:**  
Okay. And read optimized. Basically it's structured so people can easily access and use the data. It's designed for consumption, not just storage. Thinking about that read optimization often really pushes teams to consider how people will use it.

<div align="right">

> **Speaker 2:**  
Makes sense. Standardized. Built to play well with others, common form, as common understanding. So it fits into the broader ecosystem.

</div>

> **Speaker 1:**  
And the last part. User needs. That sounds crucial.

<div align="right">

> **Speaker 2:**  
Absolutely fundamental. It's not data for data's sake. It's built to solve a problem or answer a question for someone who needs that data.

</div>

> **Speaker 1:**  
So it's a very deliberate approach then. Not just, you know, dumping data somewhere. There's a philosophy.

<div align="right">

> **Speaker 2:**  
Precisely. That's the data as a product mindset. Think about any other product a company makes, like software or even a physical thing.

</div>

> **Speaker 1:**  
Okay. You wouldn't just hand over raw materials.

<div align="right">

> **Speaker 2:**  
Yeah. Right. You design it, make it user friendly, reliable, make sure it actually delivers value.

</div>

> **Speaker 1:**  
Right. You package it, support it.

<div align="right">

> **Speaker 2:**  
Exactly. Exactly the same thinking applies here. But for data, treated with that same care and focus on the consumer.

</div>

> **Speaker 1:**  
Okay. So if we're treating it like a product, what are the essential features, the key attributes that make it, you know, a product?

<div align="right">

> **Speaker 2:**  
Good question. There are several key characteristics. First off, it has to be discoverable.

</div>

> **Speaker 1:**  
Findable.

<div align="right">

> **Speaker 2:**  
Yeah. People need to be able to find it easily, usually through something like a data catalog.

</div>

> **Speaker 1:**  
Okay. Then, addressable.

<div align="right">

> **Speaker 2:**  
It needs a unique, stable identifier like a web address. So you can always point to it. Got it. Trustworthiness and truthfulness are huge. You need to know you can rely on it.

</div>

> **Speaker 1:**  
How do you ensure that?

<div align="right">

> **Speaker 2:**  
That comes from clear ownership, knowing who's responsible, understanding its lineage, where the data came from, what happened to it, and having clear quality metrics readily available.

</div>

> **Speaker 1:**  
Transparency.

<div align="right">

> **Speaker 2:**  
Exactly. And also needs to be self-describing. It's timing. It comes with its own explanation. Good metadata, clear documentation, and something called a data contract will probably dig into that more later, which defines its structure, its terms of use.

</div>

> **Speaker 1:**  
Okay. What else?

<div align="right">

> **Speaker 2:**  
Interoperability. Using standard formats, so it can connect and work smoothly with other data products. And of course, security is not negotiable. Plus, adherence to governance rules.

</div>

> **Speaker 1:**  
Right. And it's really important to stress just making raw data available, maybe in a bucket somewhere, without all this context metadata governance. That's not a data product.

<div align="right">

> **Speaker 2:**  
Okay. Clear distinction.

</div>

> **Speaker 1:**  
So this all sounds like quite a big shift from how organizations traditionally handled data. What prompted this? Why data products? What problems are they solving?

<div align="right">

> **Speaker 2:**  
Yeah, it's a major shift. And it leads us straight into the whole idea of the data mesh.

</div>

> **Speaker 1:**  
Ah, the mesh.

<div align="right">

> **Speaker 2:**  
Okay. Historically, you had these big centralized data architectures. Data warehouses, later data lakes.

</div>

> **Speaker 1:**  
Yeah, the monolithic approach.

<div align="right">

> **Speaker 2:**  
Right. And they served a purpose, definitely. But as data just exploded, the volume, the variety, the speed, these central systems often became bottlenecks. Too slow, too overloaded.

</div>

> **Speaker 1:**  
Exactly. Request pile-up. The central team gets overwhelmed. They don't always have the deep context for all the different types of data. It just doesn't scale well in really complex data-rich organizations.

<div align="right">

> **Speaker 2:**  
These systems often just couldn't keep up with how fast business units needed things.

</div>

> **Speaker 1:**  
So the data mesh is the alternative?

<div align="right">

> **Speaker 2:**  
It's a fundamentally different model. It's decentralized, organized around business domains.

</div>

> **Speaker 1:**  
Decentralized. Okay. That makes intuitive sense for a big company. How did data products fit into that decentralized picture then?

<div align="right">

> **Speaker 2:**  
They're kind of the core building blocks. Yeah. In a data mesh, those individual business domains, like say marketing or sales or logistics, they take ownership of the data they generate and understand best.

</div>

> **Speaker 1:**  
Right. The people closest to the data.

<div align="right">

> **Speaker 2:**  
Precisely. And the data that audits are the tangible, shareable units of data that these domain teams create, manage, and offer out to other teams. So the marketing team makes a customer interactions data product. The sales team makes a pipeline data product. Something like that.

</div>

> **Speaker 1:**  
Exactly. The idea is who knows sales pipeline data better than the sales domain team? They're best placed to package it up reliably for others to use.

<div align="right">

> **Speaker 2:**  
Okay. That clicks. Can you give a more concrete example? Maybe make it really tangible?

</div>

> **Speaker 1:**  
Sure. Let's use the user registration example from data mesh in action. Imagine a company, they have a system where users sign up.

<div align="right">

> **Speaker 2:**  
Okay. Standard stuff. In the old world, maybe a central analytics team needs data about user demographics. They'd have to go ask the engineering team that runs the registration system, figure out the tables, extract it. It's kind of an afterthought for the registration team.

</div>

> **Speaker 1:**  
That's data as a byproduct.

<div align="right">

> **Speaker 2:**  
Right. Extra work for them. Potential delays for the analytics team.

</div>

> **Speaker 1:**  
Exactly. Now, in a data mesh world, the team responsible for user registration owns that user data. They would proactively design and offer a registered user's data product. It would be well-defined, maybe offering key demographics, sign updates, in a clean, documented format.

<div align="right">

> **Speaker 2:**  
The marketing team, wanted to analyze user trends, could just connect to this readily available data product.

</div>

> **Speaker 1:**  
Much smoother. They self-serve. Less back and forth, less reliance on the original team for explanations or custom extracts.

<div align="right">

> **Speaker 2:**  
And what we often see is that this direct ownership leads to higher quality, more relevant data products, because the domain team cares about it.

</div>

> **Speaker 1:**  
That makes a lot of sense. So it really is the domain teams, the ones who get the data who are building these products.

<div align="right">

> **Speaker 2:**  
Lisa Sice, that's the principal, domain-driven ownership. The teams that understand it, use it daily. They are accountable for building, maintaining, and improving the data products for their area.

</div>

> **Speaker 1:**  
Okay, so what actually goes into one of these data products? It's clearly more than just the data set itself. What are the components?

<div align="right">

> **Speaker 2:**  
Absolutely more. Think of it like a package service, or a well-defined component. You've got the data itself, of course. But critically, you have output ports.

</div>

> **Speaker 1:**  
Output ports.

<div align="right">

> **Speaker 2:**  
Yeah, these are the defined ways consumers can access the data. Read only access points. Could be SQL tables, API endpoints, files in specific formats. Define ways to get the data out.

</div>

> **Speaker 1:**  
Okay, make sense. It might also have input ports. If it needs to ingest data from specific upstream sources, then there's a crucial discovery port.

<div align="right">

> **Speaker 2:**  
For finding it. Exactly. This hooks into the data catalog. It provides all the metadata, what the data means, who owns it, quality scores, how fresh it is, all that descriptive stuff.

</div>

> **Speaker 1:**  
So you know what you're getting.

<div align="right">

> **Speaker 2:**  
Right. Clear ownership info is vital too. And then under the hood, you've got the actual code that does the transformations.

</div>

> **Speaker 1:**  
The pipeline logic.

<div align="right">

> **Speaker 2:**  
Yeah, the code that cleans, reshapes, aggregates the data. Plus the underlying data storage, which is often kept separate, isolated for that specific product. Keeps things tidy.

</div>

> **Speaker 1:**  
You also need automated tests. Super important for ensuring data quality. And good documentation is essential.

<div align="right">

> **Speaker 2:**  
Of course. And depending on the product, you might also find other bits, like cost management components, governance policies actually embedded as code, CICD pipelines for automated testing and deployment, observability tools to monitor how it's running.

</div>

> **Speaker 1:**  
Wow. Okay. So it's quite a sophisticated little package.

<div align="right">

> **Speaker 2:**  
It can be. Yeah. It's designed to be robust and trustworthy.

</div>

> **Speaker 1:**  
With all those components and considerations, designing one must be quite involved. Is there a structured way to approach it? A framework?

<div align="right">

> **Speaker 2:**  
Yes, definitely. A really popular tool that's emerged is the data product canvas.

</div>

> **Speaker 1:**  
A canvas, like for brainstorming.

<div align="right">

> **Speaker 2:**  
Kind of, yeah. It's a visual framework, usually a one-pager, that helps teams collaboratively think through and design their data product. It forces you to answer key questions up front.

</div>

> **Speaker 1:**  
What sort of questions? What are the main parts of this canvas?

<div align="right">

> **Speaker 2:**  
It typically has around eight key building blocks. You start with the basics, and a domain it belongs to, and a clear data product name. Then maybe the most crucial part, defining the consumer and their specific use case. Who is this for? What problem are they trying to solve with this data? Getting this right is vital.

</div>

> **Speaker 1:**  
Understanding the why.

<div align="right">

> **Speaker 2:**  
Exactly. Then you define the data contract. This is the promise where the data will look like the schema, quality levels, service level agreements, SLAs. The formal agreement.

</div>

> **Speaker 1:**  
Yep. You identify the data sources, where does the raw information come from, and map out the data product architecture. The high level steps, the pipeline, the tech involved in creating it.

<div align="right">

> **Speaker 2:**  
Okay. The canvas also pushes you to define a ubiquitous language, common terms, everyone agrees on, business and technical folks. And finally, a classification is this raw data. Clean data, aggregated data, helps users understand its nature.

</div>

> **Speaker 1:**  
That sounds incredibly useful for getting everyone on the same page.

<div align="right">

> **Speaker 2:**  
It really is. And teams that use tools like this rigorously, often find they have a much clearer, shared understanding, especially those user needs, which leads to way more successful products.

</div>

> **Speaker 1:**  
And it sounds like it has to be a team effort right from the start.

<div align="right">

> **Speaker 2:**  
Oh, absolutely. It's designed for collaboration. You need the business users who know the needs, the data product managers steering the ship, maybe governance folks, ensuring compliance, and obviously the data and platform engineers will build it. They'll talk in together.

</div>

> **Speaker 1:**  
Mm-hmm. And it's usually iterative. You don't carve it in stone on day one. You design maybe build a small version, get feedback, refine it. Learn as you go.

<div align="right">

> **Speaker 2:**  
Okay. Now, you mentioned data pipelines as part of the architecture. Where do they fit in this whole picture? They seem pretty central to actually making the data product work.

</div>

> **Speaker 1:**  
They are absolutely fundamental, your spot on. Pipelines are the engines the circulatory system that creates and moves the value within the data product.

<div align="right">

> **Speaker 2:**  
We do the heavy lifting. Pretty much. They cover those key stages. Ingestion, getting data from the sources, transformation, cleaning it, shaping it, joining it, and reaching it. And making that final, polished data available through those output ports we talked about.

</div>

> **Speaker 1:**  
And nowadays, you have tools like AirBite or 5-Tran that offer loads of pre-built connectors, which really speeds up that ingestion part, makes connecting to different sources much faster.

<div align="right">

> **Speaker 2:**  
Standardization helps there.

</div>

> **Speaker 1:**  
Definitely. And a really key best practice that's emerged is this idea of shift left data quality.

<div align="right">

> **Speaker 2:**  
Shift left, like in software testing.

</div>

> **Speaker 1:**  
Exactly the same idea. Embed data quality checks and validation as early as possible in the pipeline, ideally right after ingestion, or even at the source. Catch problems early.

<div align="right">

> **Speaker 2:**  
Right. Don't wait until the data is landed in the final table to find out it's wrong. Fix it, or at least flag it, much closer to the source.

</div>

> **Speaker 1:**  
Saves a lot of pain downstream.

<div align="right">

> **Speaker 2:**  
Makes perfect sense.

</div>

> **Speaker 1:**  
Okay, so we have all these domain teams, potentially dozens of them, building their own data products using pipelines. How do you stop it becoming, well, chaos? Everyone reinventing the wheel, using different tech stacks.

<div align="right">

> **Speaker 2:**  
Ah, yes, the reinventing the wheel problem. That's a major reason why the concept of a self-served data platform is so critical in a data mesh.

</div>

> **Speaker 1:**  
A platform, okay, what is that view?

<div align="right">

> **Speaker 2:**  
The core idea is simple. You don't want every single domain team having to figure out, say, the best way to ingest data from Salesforce, or how to manage scalable data storage, or set up monitoring. These are complex, specialized skills.

</div>

> **Speaker 1:**  
Yeah, that would be hugely inefficient.

<div align="right">

> **Speaker 2:**  
Totally. So the self-served platform centralizes those common specialized capabilities. It provides the infrastructure, the tools, the standards, that all domain teams can then use to build their data products.

</div>

> **Speaker 1:**  
So it's like a shared foundation? Or a toolkit?

<div align="right">

> **Speaker 2:**  
Exactly. It takes those tricky, duplicated tasks, infrastructure management, security enforcement, maybe providing standard pipeline orchestration tools, and puts them into a dedicated platform team.

</div>

> **Speaker 1:**  
But crucially, the domain teams still build their own products.

<div align="right">

> **Speaker 2:**  
Yes. The goal is self-service, maximizing the autonomy of those domain teams. The platform empowers them. It doesn't dictate the specifics of their data product logic. It just gives them the reliable tools and guard rails to do efficiently and consistently.

</div>

> **Speaker 1:**  
What are the key features of such a platform?

<div align="right">

> **Speaker 2:**  
Well, fundamentally, it used to provide stable, reliable data infrastructure. Clear boundaries between teams, often called tenancy. So one team's work doesn't mess up another's. Isolation.

</div>

> **Speaker 1:**  
Right. And key shared resources, storage, compute, networking. Often you see things like bundles, which are pre-packaged sets of resources a team might need to deploy a data product. Makes deployment easier. And there's usually utility playing on top. This offers things like declared as specifications, teams say what they want. The platform figures out how maybe single-command deployments automatic registration of new products and the data catalogs, stuff like that.

<div align="right">

> **Speaker 2:**  
Streamlining the process for the domain teams. That's the aim. Reduce friction, increase speed and reliability will keep that domain ownership intact.

</div>

> **Speaker 1:**  
Okay. You mentioned data contracts earlier, and they sounded important, especially for making these different products work together. Can we dig into those a bit more? Why are they so crucial?

<div align="right">

> **Speaker 2:**  
Absolutely. Data contracts are, well, they're a fundamental glue in a data mesh. You really can't overstate their importance.

</div>

> **Speaker 1:**  
Okay. So what is the data contract formally?

<div align="right">

> **Speaker 2:**  
Think of it as a formal agreement, a documented promise between the data product producer, the domain team, and the consumers of that data product.

</div>

> **Speaker 1:**  
An SLA for data.

<div align="right">

> **Speaker 2:**  
Kind of, but richer. It defines the interface of the data product. It specifies the schema, the fields, the data types. It includes metadata definitions, business terms. It lays out the terms of use, the quality expectations, maybe freshness guarantees. It covers the data model and the semantics, what the data actually means.

</div>

> **Speaker 1:**  
So everyone knows exactly what they're getting and how they can use it.

<div align="right">

> **Speaker 2:**  
Precisely. It sets crystal clear expectations, and this has huge benefits.

</div>

> **Speaker 1:**  
Such as?

<div align="right">

> **Speaker 2:**  
Well, first, trustworthiness. Consumers know what to expect, and the contract provides a basis for holding the producer accountable. Second, interoperability. If everyone adheres to clear contracts, connecting products becomes much easier. Less guesswork, fewer integration headaches.

</div>

> **Speaker 1:**  
Exactly.

<div align="right">

> **Speaker 2:**  
And third, managing change. This is massive. If a producer needs to change the data product, maybe add a field, change a format, the contract is the mechanism for communicating that change before it happens.

</div>

> **Speaker 1:**  
Ah, so consumers don't suddenly find their processes breaking.

<div align="right">

> **Speaker 2:**  
Right. The contract allows for versioning and clear communication preventing downstream chaos. And those output ports we mentioned earlier, they are formally defined in the data contract. With format, JSON, Parquet, with protocol, API, JDBC, it's all specified there.

</div>

> **Speaker 1:**  
Okay, so contracts are key for smooth operation. Now, we've got these well-defined contract bound data products being built on a platform. How do we actually know if they're any good? Are they successful? Delivering value.

<div align="right">

> **Speaker 2:**  
Yeah, this is a what question. That's where metrics come in. Measuring this success is absolutely essential.

</div>

> **Speaker 1:**  
Why? Just to prove their worth.

<div align="right">

> **Speaker 2:**  
Well, partly, yes, to demonstrate impact, but also critically to guide future development. You need feedback to know what's working, what's not, where to invest effort next.

</div>

> **Speaker 1:**  
Makes sense. So what kind of things do you measure?

<div align="right">

> **Speaker 2:**  
We generally look at a few key dimensions.

</div>

> **Speaker 1:**  
Huh.

<div align="right">

> **Speaker 2:**  
First, usage and adoption. Pretty straightforward. Are people actually using this thing? Like, number of users. Queries run.

</div>

> **Speaker 1:**  
Exactly. Daily or monthly active users, frequency of use, maybe volume of data pulled.

<div align="right">

> **Speaker 2:**  
Yeah, also things like time to value for new users. How quickly can someone new start using it effectively?

</div>

> **Speaker 1:**  
Okay. Usage. What else?

<div align="right">

> **Speaker 2:**  
Second and arguably most important. Value and business impact. Is this data product actually moving the needle for the business?

</div>

> **Speaker 1:**  
How do you measure that? It sounds harder.

<div align="right">

> **Speaker 2:**  
It can be, but it's crucial. You try to tie it to tangible outcomes. Did using this product lead to increased revenue? Did it help save costs by improving efficiency? Did it save employees time by enabling faster decisions or automating tasks?

</div>

> **Speaker 1:**  
Real business outcomes.

<div align="right">

> **Speaker 2:**  
Right. Then third, data quality. We talked about contracts promising quality. So you need metrics to track that. Consistency, accuracy, completeness, timeliness of the data. Are we meeting the promises?

</div>

> **Speaker 1:**  
Okay. Quality. Anything else?

<div align="right">

> **Speaker 2:**  
Fourth is often technology and operations. How reliable and efficient is the product itself? Things like uptime, latency of queries, but also DevOps style metrics for the team building it. Cycle time. How long does it take to go from an idea for a feature to deploying it? Deployment frequency. How often can we safely release updates? Mean time to recovery. If it breaks, how fast can we fix it?

</div>

> **Speaker 1:**  
So usage, business value, quality and operational efficiency. A pretty rounded view.

<div align="right">

> **Speaker 2:**  
Exactly. And the key is always to align these metrics back to the business objectives. Why did we build this data product in the first place? The metrics should reflect that goal. Focus on outcomes, not just outputs like a number of pipelines built.

</div>

> **Speaker 1:**  
Right. Impact over activity.

<div align="right">

> **Speaker 2:**  
Precisely. Sometimes people frame it using lenses like the customer dimension, user satisfaction, solving their problem. The technology dimension, those operational metrics. And the business dimension, revenue, cost, time savings.

</div>

> **Speaker 1:**  
Any specific techniques like surveys?

<div align="right">

> **Speaker 2:**  
Yes, surveys can be great. A simple product market fit survey, asking users, how disappointed would you be if this data product disappeared? Can be surprisingly insightful. If lots of people say very disappointed, you know you're providing real value.

</div>

> **Speaker 1:**  
Interesting. OK, one final but really important piece, governance. I.E.S. governance. Can't forget that. With all these decentralized teams building products, how do you maintain order? Ensure security, compliance, consistency across the whole organization? It sounds like it could get messy without some oversight.

<div align="right">

> **Speaker 2:**  
It definitely could. And that's where the idea of federated computational governance comes in. Federated.computational.governance. OK, let's unpack that. It's about striking a balance. You want the domain teams to have autonomy to move fast and know on their products. But the organization still needs global standards. Security rules, privacy regulations like GDPR or CCPA, standards for interoperability so products can connect.

</div>

> **Speaker 1:**  
So you can't have complete anarchy?

<div align="right">

> **Speaker 2:**  
Yeah, absolutely not. Federated governance means you don't have one central team dictating everything that's the old bottleneck model. Instead, you distribute governance responsibilities.

</div>

> **Speaker 1:**  
How does that work?

<div align="right">

> **Speaker 2:**  
You have a central body that defines the global rules, the baseline standards, the policies everyone must adhere to. But the enforcement and implementation of many of those policies within the context of a specific data product can be delegated to the domain teams.

</div>

> **Speaker 1:**  
So shared responsibility.

<div align="right">

> **Speaker 2:**  
Exactly. Global standards, local implementation and accountability. In the computational part, that refers to automating these policies as much as possible.

</div>

> **Speaker 1:**  
Policies as code?

<div align="right">

> **Speaker 2:**  
Yes. Instead of just writing rules in a document, you express them in code that can be automatically checked and enforced. For example, code that automatically scans data for PII and applies masking rules or checks if the product's metadata meets the required standard before it can be published.

</div>

> **Speaker 1:**  
Makes governance scalable and consistent.

<div align="right">

> **Speaker 2:**  
That's the goal. Less manual checking, more built-in automated guardrails. It supports autonomy while ensuring compliance.

</div>

> **Speaker 1:**  
Okay, that makes sense. And guiding each individual data product who's ultimately responsible for its direction and success.

<div align="right">

> **Speaker 2:**  
Now it would be the data product owner. Like a product owner in agile software development.

</div>

> **Speaker 1:**  
Very similar role, yes. This person is responsible for the product's vision. What is it trying to achieve? They build and prioritize the roadmap what features get built next. And they define the success criteria. How do we know if it's valuable?

<div align="right">

> **Speaker 2:**  
So they own the what and why?

</div>

> **Speaker 1:**  
Exactly. They need a deep understanding of the consumer's needs. They work closely with the domain team, the engineers, the stakeholders, to make sure the product delivers real value.

<div align="right">

> **Speaker 2:**  
A crucial linking role.

</div>

> **Speaker 1:**  
Absolutely. They're the bridge between the technical team building the product and the business users or other data consumers who rely on it. This has been incredibly illuminating, really clarified how all these pieces fit together.

<div align="right">

> **Speaker 2:**  
So just to quickly recap the big takeaways for everyone listening.

</div>

> **Speaker 1:**  
Yeah, I think the core is data products are these self-contained, autonomous user-focused units of data. They're absolutely central to making a decentralized data mesh architecture actually work.

<div align="right">

> **Speaker 2:**  
And they aren't just raw data.

</div>

> **Speaker 1:**  
No way. They require careful design, maybe using something like the data product canvas. They're built on shared, self-serve platforms to avoid reinventing wheels. They rely heavily on clear data contracts for trust and interoperability. And you need to measure their success.

<div align="right">

> **Speaker 2:**  
Definitely. Using metrics across usage, value, quality, and operations, all operating within that federated governance framework with clear ownership by a data product owner.

</div>

> **Speaker 1:**  
So for you listening, hopefully this deep dive gives you a much clearer picture of data products in the mesh. It really comes down to a different mindset, doesn't it? Treating data with real intention, focusing on who needs it and why.

<div align="right">

> **Speaker 2:**  
It really does. And it makes you wonder, doesn't it? If you started applying this data as a product, thinking in your own organization or your field, how could that change things? What new possibilities open up when data isn't just a byproduct, but something designed, packaged, and delivered with the user truly in mind?

</div>

> **Speaker 1:**  
That's a powerful thought to leave people with.

<div align="right">

> **Speaker 2:**  
Definitely something to chew on. If you want to explore these ideas further, we absolutely recommend checking out the resources we mentioned earlier. Data mesh and action, the architecture books, the articles. Lots more detail there.

</div>

> **Speaker 1:**  
Absolutely. Keep digging. Thanks so much for joining us for this deep dive.
