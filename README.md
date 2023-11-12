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


```bash
no code yet
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)