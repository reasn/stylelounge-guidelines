# Pull Requests

Pull requests are a key part of the development process at StyleLounge. We do them for every change. They are a form of asynchronous pair programming and they should hopefully help us spot bugs and design mistakes in our code before our users do.

Doing reviews for other people's code is an **essential** part of every developer's job.**It is one of the highest priority things you can work on**. Every open pull request we have is a change that isn't shipping to users. Since we often need multiple attempts at a new feature to get it just right for our users that means the longer PRs take the longer it takes us to get polished features completed.

## Submitting pull requests

#### Review your own code

You should read over your own code, make sure you didn't omit any files, check for style errors and so on. You should do this before you create the PR.

#### Keep your changes small

Small changes are much **easier to review**. They're also much easier to explain to people. This means that **mistakes are less likely** to sneak through and the discussion of the change should be much more productive. It also means your PR should avoid ending up with tens of comments that go round and round in circles without ever getting your code merged. It is not always possible to break a change up into small parts but it very often is.

A good guideline for this is that your change should not effect a combined total of more than 400 lines.

#### Write good descriptions

The title of the PR should include the reference for any tickets covered by this change. You may also want to copy the description from the ticket into your description. The description for your PR should tell the story of your change in a clear and concise way. It should explain both **why** you are making this change and **what** you changed. Not all reviewers will have a deep knowledge of that part of the system so you must make it possible for them to provide useful insight. This means explaining what the existing behaviour was, how you changed it, and why this was thought to be useful.

#### Write good commit messages

Your commits should be logically separate changes. This means that you should aim to separate things like lint cleanups from actual behaviour changes. They should have good commit messages that explain what was changed at each step.

#### Respond quickly

You shouldn't go off and get stuck into something else while you have PRs open. This makes the reviews less effective for everyone because everyone will now need to switch context more frequently. You will need to remember what was going on in your change, they will need to familiarise themselves with what was going on when they raised a comment. **If you have a PR open your number 1 priority should be getting it reviewed and merged.**

#### Pair review

If you're working on a component or a service that others are not familiar with then offer to do an in-person pair review with someone. This guarantees you'll get eyes on your changes and get your code through the door quicker. It's also a great way for knowledge sharing and teaching people new techniques.

## Reviewing code

#### Know what you need to review

Because getting PRs merged quickly is so important you need to stay on top of the changes people want your input on. Follow your team's slack channel as well as \#dev-only and \#dev-scrum-teams.

#### Respond quickly

Tolerate being interrupt driven. You need focussed time to your other work done but PRs are time sensitive because they block other people. You should never put off code review for more than a few hours.

#### Prioritise code review highly

**It's one of the most important things you can work on**. The only things that should come ahead of it are time critical work such as fixing availability problems or dealing with blockers. This means you should expect to spend some time every day reading other people's code.

#### Be thorough

Reviewing code is hard and error prone. It is our last line of defense against downtime and tech debt. **You must pay attention, ask questions and not approve lightly**. Sometimes you will slip and miss something or only notice late in the review process. Not great but it is forgiven. Own up to it and move on. Confused about a bit of code? Ask what it does - **there are no stupid questions**.

#### Don't block progress

While code reviews need to be done thoughtfully and thoroughly we also need to avoid blocking progress. This means you should help people with solutions, not only identify problems. Often it might be faster to go and pair with someone for a bit to get their code tidied up instead of going back and forth on GitHub about it.

### Things to look for

#### Clarity

Things should be named well and should be easy to follow when reading. The code should attempt to be self documenting.

#### Correctness

There must be unit tests. They should test the edge cases. The code should behave as the submitter described. The code should use other APIs correctly.

#### Our style

It's important that code changes to our application conform with our guidelines. Also they should make intentional decisions about whether to use our patterns and best practices. It's important to care for consistency and quality.

#### Performance

The code should perform within our targets for a particular area. It should not use obviously suboptimal algorithms. Simpler code is often faster.

This has been revised and taken from our international competition 😜 \(github.com/lyst/MakingLyst/tree/master/code-reviews\)

