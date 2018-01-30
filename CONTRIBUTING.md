# Contributing to the Project

Bug reports and feature requests are always welcome,
but code is even better!


## Development

Set up your environment
with the appropriate development dependencies:

```
yarn
```

As you work...

- Add or update any appropriate unit tests
  in the `test` directory,
  and make sure all tests are passing with `npm test`
- Add your changes to the [changelog](CHANGELOG.md)
- Update or add inline documentation
  using [SassDoc][sassdoc] as appropriate,
  and compile the docs with `gulp sassdoc`

[sassdoc]: http://sassdoc.com/


## Committing

Linting, testing, and documentation
should be done before every commit:

```bash
npm run commit
```

They can also be triggered individually:

```bash
# lint
gulp sasslint

# test with mocha/true
npm test

# compile docs
gulp sassdoc
```

Once you've fixed any final errors or typos,
commit your changes, and submit a pull request!


## Pull Requests

We use the `master` branch for production-ready code,
and side-branches for everything in-progress
or up-for-debate.

When submitting a patch via pull request:

- Write a clear, descriptive commit message
- Keep it simple: one bug fix or feature per pull request


## Code of Conduct

As a company,
we want to embrace the very differences
that have made our collaborations successful,
and work together to provide the best environment
for learning, growing, working, and sharing ideas.
It is imperative that [OddBird][oddbird] continue to be
a welcoming, challenging, fun, and fair place to contribute.

See our [Code of Conduct][coc] for details.
We also recommend following the [Sass community guidelines][sass].

[oddbird]: http://oddbird.net/
[coc]: http://oddbird.net/conduct/
[sass]: http://sass-lang.com/community-guidelines
