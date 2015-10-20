# Learn Function Programming in JavaScript with Node.js

Do you want to learn functional programming but don't want to learn a whole
new language?

If so then this is the repo for you! I am thinking about making this a book
but for now this will just be an outline and a bunch of exercises you can
work though.

Each chapter will cover a part of learning function programming. Though it is
meant to work through in order you can feel free to work through it in any
order. If I reference something from a previous chapter I will put a link to it.

This project expects that you understand a basic node.js and and how to use
git. If you need to learn more about these checkout the following.

*   **Learn basic Node.js:** [NodeSchool learnyounode](http://nodeschool.io/#workshoppers)
*   **Learn more about git:** [Github Code School](https://try.github.io/)

## Get Started

To get started with the exercises you should first fork this repo. This will
let you check in your work on your own repo as well as send me pull requests
back for bugs and fixes. ;)

Once you fork it you should clone it locally like this:

```bash
git clone https://github.com/[Your Github username]/learn-functional-programming.git
cd learn-functional-programming
npm install
```

This is the first four steps in almost any open source Node.js project. You
almost always want to first fork the repo, clone it locally, move into the
folder, and do a npm install to install all the dependencies.

All the exercises are in the exercises folder and they have a number, chapter,
and a name.

Now if you run the following you will see all the breaking tests for all
exercises.

```base
npm test
```

This is nice to see, you should see all failing tests but this can be a lot
to see all at once. If you want to just run one test at a time when you work
on them you can add a .only to the it function in each exercise.

Here is an example test:

```javascript
describe('This is an example tests', function() {
  it('This is the test I am working on.', function() {
    // This is my test exercise
  });
});
```

Now to run only this test on npm change it to this:

```javascript
describe('This is an example tests', function() {
  it.only('This is the test I am working on.', function() {
    // This is my test exercise
  });
});
```

The only tells mocha to only run that one test. Once you are done don't forget
to remove it. If you add it to to more then one place it will just run the last
one it finds and there is no guaranty on the order your tests run.
