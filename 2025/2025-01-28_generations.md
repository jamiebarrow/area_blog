# 2025-01-28 - Generations

History repeats itself.

That is a well known saying in society.
In the software engineering field this is also true: it tends to repeat itself around every decade.
Some examples I've seen are going back and forth between thin-client and thick-client applications.
Or recently, with the Cloud switching between paying for self-hosting versus paying for time and compute resources of external hosting services.

Sometimes the frequency of change is faster, sometimes shorter.
But if any industry was a fashion industry, it would be the computer industry.

As software developers, we don't ask about what is "on trend this season", especially when talking about something most people think is boring, such as Linux.
There are equivalent phrases though, such as "buzz word", and likely others.

The buzz word these days is Artificial Intelligence.
AI is penetrating every other industry just like the Internet has done before.
In the past, businesses were racing to have their own online presence.
Well, not so much once the dotcom bubble burst back in the '90s.

Back in the '90s you were trendy if you had the Nokia 3310.
What a clean form factor.
I remember kids in my class hiding their phones away from the teacher while they tried to get the high score on snake.
If you didn't have it you weren't cool, man.
Which kids these days won't understand, I mean, it didn't even have a colour screen!

Come to think of it, maybe that was even a 2000's thing.
The 90's was more about Nike sneakers, Chicago Bulls t-shirts and listening to Nirvana.
I still listen to Nirvana, but I digress.

Once society moved on from the desktop Internet and from Nokia, they moved onto the new fad of smart phones and the mobile Internet.
The iPhone was on trend once Steve Jobs introduced it back in 2007.
Just under a decade after the Nokia 3310.

Every company didn't just want an online website presence, they wanted an App.

> "You're a developer? Can you build an app for me?"
>
> "No, sorry, I likely can, but it's not my expertise, so it's likely better you find someone who has it as their strength."

Skipping through time a bit, we noticed Bitcoin popping up.
Blockchain seemed to be all the rage with Bitcoin and its various bubbles and fashionista wannabe variants.
Everyone thought Bitcoin and blockchain would change the world, and "give it to The Man".
Even banks and governments seemed to try adopt the underlying blockchain technology, to try reduce costs.
Even the Hawk Tuah girl ran her own scam blockchain recently to get rich quick.
So in reality, not that much has really changed.

Blockchain wasn't the easiest for just anyone to use, you had to become a real geek of the blockchain to use it successfully without making too many mistakes.
People could still get scammed if not knowledgable enough.
It seems its still not yet blockchain's time for the general public.
Maybe in the future, we don't know.

It reminds me a bit about the '90s again.
Kids were the ones using VCR's and showing their parents how to work the remote control.
It's a generational thing.
Kids just had more time to play with it.

And that's the thing: success is not quick, for most it takes time and effort.

Success doesn't just come overnight.
It takes years of commitment, research, planning, hard work, sacrifices and so on until the eventual "overnight success".
There are various people attributed to the saying, but I enjoy this one even though I'm not the biggest football fan:

> "I start early and I stay late, day after day, year after year,
>  it took me 17 years and 114 days to become an overnight success"
>
> -- Lionel Messi

I can relate to that, having invested a lot of time on learning about computers.
Especially when I think back to the weekends spent in high school where I was on the Internet on Friday night learning about Visual Basic instead of socializing.
I enjoyed it, and I didn't see it as an investment.
It was a passion.

After high school I went to the University of the Witwatersrand in Johannesburg, South Africa.
From 2003 to 2005 I did my Bachelor of Science (BSc), and in 2006 continued with my Honours in Computer Science.
There were various computer science modules over the years, and my favourite ones were the difficult ones related to algorithms and data structures.

There's a problem named the Travelling Salesman Problem (TSP), which is likely one you would encounter every day in real life.

Imagine you worked for a fast food delivery service and had to get the orders out hot and fast throughout the neighbourhood.
If it's only a few orders, the fastest route isn't always important.
If you're on a bicycle it might be easier, an e-bike, even quicker.

Experience teaches you the short-cuts.
In the worst case, a delivery is late or wrong, and its easy enough to solve: send another pizza, or credit/refund the customer.
Don't send the new guy on complex orders if you don't have to.
Simple enough.

But perhaps you're a larger multi-national courier service and you have certain service level agreements to hold up to.
Failure resulting in huge delays, expenses and possible legal issues.
Finding the optimal route becomes a lot more important in this case.

The navigation systems we have today that made the map books of the past irrelevant, weren't just overnight successes.

They likely all also are solving some form of the Travelling Salesman Problem (hence the name of the problem).

The TSP typically involves Graph Theory algorithms.
You can think of all the destinations and turning points and other points of interest as a graph, each point being called a node.
Destination A being one node in the graph and destination B another node.
A route between them, means you have a line connecting these nodes.
That path could be straight, or very jagged, connecting many other points of interest.

If you consider all the various points of interests and routes between two points, you likely end up with a huge spider web of connections.
Finding the best route, is trying to solving the Travelling Salesman Problem.

It starts to become combinatorial in the number of possibilities, and the TSP is what's known as a "hard problem" in Computer Science.
Either it becomes difficult to say exactly how long the problem will take to be solved, or it takes too much computing power and too much time to solve, so it's not worth waiting for that perfect answer.

Instead, an approximation is likely easier and quicker to get a solution, even if its not fully correct.
We do this all the time when commuting, we likely make use of some strategies depending on the day:

- take the highway outside of rush hour
- accept the longer travel time, and take the highway anyway
- ignore routes with accidents
- take the quickest route, its more effective
- today it seems less busy and we have time, lets take the scenic route, its more enjoyable

These seem pretty intuitive, and the chosen strategy may depend on our own past experiences and preferences.
For someone who's always had bad luck and taken longer on the highway, they may try to take routes that avoid the highway.
It's just a strategy, it's never necessarily going to be the best way.
It's what computer scientists call a "heuristic".
It's a best guess, but guesses still stand a chance to be wrong.

One algorithm for finding a route through a network is the A-Star (A*) Search Algorithm.
It was published in a paper titled "A Formal Basis for the Heuristic Determination of Minimum Cost Paths"
by Peter Hart, Nils Nilsson and Bertram Raphael, in the journal of the IEEE Transactions on Systems Science and Cybernetics.
It uses heuristics to attempt at being more efficient in finding a shortest path than similar approaches.

This was back in 1968.
The field of AI is said to have started back in the 50s.
There is even a movie based on the story of Alan Turing's "The Imitation Game" which was documented in the paper "Computing Machinery and Intelligence".
This was published in the journal "Mind" back in October 1950.

After helping in World War II to decode encrypted messages being sent from the Enigma machine, he later put forth the question: can computers think?
The Turing Test is more around seeing if you can involve a human in a conversation, unaware that they are in fact conversing with a computer and not a human.
The paper from Turing is now 75 years old, a grandpa, so to say.
The TSP could even be said to trace back to the 1850s when Irish mathematician William Rowan Hamilton introduced a similar problem.

If I think to our ancestors being on the move and trying to find resources to survive, I would say that optimization problems are likely as old as life itself.
Solutions known to one generation, may have been known to those before them, just re-discovered, re-phrased, or solved using different approached.

AI isn't new.
It's a generational thing.
It's just back in fashion.
The trends of grandpa's day are back in stores.
It's so fashionable that some people are even offering AI powered toasters... as if that's useful.

These days the big buzz words are ChatGPT, Large Language Models (LLMs), Ollama (love that pun) and OpenAI.
Organizations seem to be coming out with products that are indeed making people feel like they're having a conversation with a human, even though they are very aware that they are talking to a computer.

I used to be a fan of traditional art over computer based techniques, because of the process, the experience.
But I find MidJourney has improved my experience in creating images based on my own thoughts and ideas.
At times, I find it even guides my creative process.
I use MidJourney as a creative tool, because it just makes it so much faster and easier.
This was likely not the case back in the 50s.

Another pun incoming: Generational AI.
It's dandy. It's cool. It's hip. It's boss. It's hot. It's kiff. It's fresh. It's gucci. It's lit. It's bussin'. No cap.

I see many people wondering about the future.
What will it be like?
We don't know.
It's a mystery.
What we do know is how it has been based on history and on our own experiences.
That's a pearl of wisdom from Jim Rohn.
Everything happens in cycles, just as the seasons: winter, spring, summer, autumn.

> Do not be deceived: God cannot be mocked. A man reaps what he sows.
> Whoever sows to please their flesh, from the flesh will reap destruction; whoever sows to please the Spirit, from the Spirit will reap eternal life.
> Let us not become weary in doing good, for at the proper time we will reap a harvest if we do not give up.
>
> Galations 6:7-9, The Bible, New International Version

You don't have to believe in the Bible or God to understand the wisdom in this passage: you reap what you sow.
You will have a good harvest during autumn, if you put the work in during the seasons prior.

Spring always follows winter. Whether an actual winter, or a metaphorical winter of disappointment.
Spring is a chance for another opportunity, so plant in the spring. Tend to your crops in the summer.
And reap your harvest in autumn.
If there is not much to harvest, that's okay. Try again next season. But it takes hard work. You only reap, what you sow.

At the end of the day, success isn't just generated.
It is created, by your own hard work.
That's how it has always been, that's how it will always be.

We don't know what will happen in the future, but if we base it on our past, it will likely involve a lot of hard work, perserverance and being diligent students to master our future.
No matter what the trends and buzz words of the day are.

We can only focus on today and ourselves.
Work to your own strengths, and build those strengths up.

What will the future look like for future generations?

The future depends on what you choose to do today.

Have a good day :)

