# Happy Fixing Bug Path Part 1

HFBP is a simple checklist anthology to support bug fixing learning path

## Checklist

#### Understand the problem

- [ ] Be here Now. Understand the problem.
- [ ] Try and reproduce the bug on local development environment, or on a test environment if the bug is requiring specific state that’s not easy to replicate.
- [ ] See the problem, understand what it should be doing, now know what I’m aiming for.


#### Consider any integration/end-to-end tests

- [ ] Consider any integration/end-to-end tests.
- [ ] If you’ve got a platform containing suitable high-level automated tests, then it might be helpful to add a new test case for this new bug.
- [ ] At the moment, this test will fail. Which is what we want, because you’ve not actually fixed the bug yet. You want this test to fail first, and then pass once the fix is in there.

#### Nail down where the change needs to be made

- [ ] Dig into the code.Depending on the solution, and depending on how well you know that codebase, this will vary in how much time and effort this will take.

> You might see a bug and immediately know where to start looking. Or you may not have a clue. Or you may know it’s not going to be a single place that contains the problem, but rather a combination of things that are working together that needs to be fixed. Obviously, each solution and each bug is different, and it’s hard to prescribe an approach that will fit all, but there are some general principles that might help. [REF](https://jamie-burns.medium.com/a-short-guide-to-fixing-bugs-in-software-764fc31bb0e5)

- [ ] Use debugging.
- [ ] Make notes. Note: the different cases you’re testing with, the areas of code you’re suspicious of, or that you’re happy are working correctly
- [ ] Make lists of things to check :)

#### Unit tests coverage

- [ ] If you’ve got unit tests as part of your solution, write some tests, focussing the specific areas of code that you’re going to be changing, and explicitly demonstrate the problem. 
- [ ] Run tests (fail).

#### Make your changes

- [ ] Be here now. Be like a surgeon — be as precise as possible, and make as few changes as I can.

>[REF](https://jamie-burns.medium.com/a-short-guide-to-fixing-bugs-in-software-764fc31bb0e5)

- [ ] Keep focus as close to the original bug as possible, and not include other fixes or improvements at the same time.
- [ ] Document other issues and raise them as new items to be reviewed.
- [ ] Run unit tests (pass).
- [ ] Run integration/end-to-end tests (pass).
- [ ] Make sure the bug itself is fixed, using the reproduction steps you initially used when investigating the bug.
- [ ] Try different manual test variations — try and break what you’ve done.

> It may be that you find different issues at the same time, in which case raise them as new issues with your product or testing teams — it may be that these related issues have already been raised somewhere else, or may be of a lesser priority, or they may be things that need to be fixed alongside your fix. Just check with your team how you want to go about it, but I would always encourage separate bugs to be documented as such, so you’ve got a full audit trail of the problems that are being fixed, even if you’re fixing them at the same time. [REF](https://jamie-burns.medium.com/a-short-guide-to-fixing-bugs-in-software-764fc31bb0e5)

#### Consider the impact

- [ ] Take a moment to consider what impact these changes will have. Look at the code you’re changing, and think about how it might behave differently now you’ve made these changes
- [ ] Also look at the impact on performance — are your changes going to cause a drop in response times, or an increase in demand on system resources?
- [ ] Finally, think about why this fix wasn’t put in when the code was first written.


#### Review your changes

- [ ] Review your changes. 
- [ ] Make sure you’ve not left in any debugging code, or extra comments

> If you can go through all your changes, and justify each one in relation to the bug you’re fixing, then you should be good to go.
[REF](https://jamie-burns.medium.com/a-short-guide-to-fixing-bugs-in-software-764fc31bb0e5)

- [ ] Re-test changes if you do end up making little adjustemnts during this review step.


#### Commit and communicate

- [ ] If possible, relate your commit to the bug item itself.
- [ ] Provide a decent commit message (make the message short and to the point, explaining why these changes are being made, not just listing the changes themselves).
- [ ] Once that’s in, development process will take over, including pull requests, gated check-ins, deployments, etc.
- [ ] Go to the bug ticket/report itself, and provide an update on findings and fixes commited.

> Documenting things like what was causing the bug in the first place is really helpful, especially if you can identify which commit the bug was introduced in, because that will help the rest of the team know how long this has been an issue for, and also maybe highlight a potential improvement to your development process to avoid similar bugs like this being introduced in the future.
[REF](https://jamie-burns.medium.com/a-short-guide-to-fixing-bugs-in-software-764fc31bb0e5)

#### Monitoring

- [ ] Keep your eye on this bug as it progresses through the different stages until it’s released to production.


```bash
no code yet ☕︎
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)