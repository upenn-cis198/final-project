## Final Project

This is the final project for the class. The goal is for you to show your knowledge of Rust to implement, or contribute to Rust in a larger project than the homework allow.
Your project should play into the strengths of Rust. That is, you must show you effectively leveraged the features of Rust to the specific program. This can be either though,
safety, parallelism, concurrency, low-level programming, performance, etc.

### Groups
You must work in teams of 3. While group projects can be annoying (lack of communication, different work styles, someone doing nothing) it is important part of software development.
Each group will have a generated Github Repository for their project. Please use this Repo to commit, and work on your code.

At the end of the semester, you will have a chance to submit anonymous feedback about your teammates. If it is determined that work was not evenly distributed, this can affect the grades for teammates who did not do enough.

### Proposal
Due: November 7th.

You and your team must submit a proposal for a project. This proposal will not be graded, but I will give you feedback about your chosen project. Your proposal does not have too be
long or detailed, but it must show that your team has a good idea for a project, complicated enough to justify a final project.

All the following are acceptable kinds of projects:
- Create a program to do some specific task. This could be:
  1) Create new Rust bindings for an existing library! If you chose this option, the binding should wrap the library in a Rustic, higher level API.
  2) An existing application rewritten in Rust.
  3) A new application altogether.
  4) A web application.
- Contribute to an existing project.
  You may be interested to contributing to some open source project in Rust. There are many crates, programs, or tools out there happy to welcome developers and contributions!
  If you're considering this option feel free to talk to me to brainstorm ideas.
- Explore deeper topics in Rust.
  There are many topics to explore in Rust! You can research/understand/use bleeding edge Rust Concepts to create, or report on something new. Examples of topics could be: constant generics, higher-kinded types, asynchronous IO, macros, something else? The biggest question with this choice: In your proposal please tell me how you're planning to do "enough" work for this option.

- There are several kinds of projects that in general will not be allow: using a machine learning library to train some classifier, using libraries for image processing, implementing most data structures. In general, these end up being boring, straightforward, and lack novelty. If you have any questions or exceptions you would like to do, please ask me.

### Requirements

- This is an exercise in software engineering, design, and implementation. A large portion of your grade will be based on this.
- Your project should have no warnings. You must use the linter Clippy, to catch lints and fix them.
- Your project must include testing: unit, property based, integration, etc.

### Grading Rubrick

1) Completeness and amount of work (50/100)
    w = average work per week for this class
    n = numbers of weeks given for the project
    p = people in your group.
    total work expected = w * n * p

    1) Complete: More than, or the expected was done for the project
    2) Somewhat: The project is below what is expected.
    3) Empty: The project is missing significant work.

2) Project Difficulty (10/100)
    1) Extensive: The project requires significant skill and work to implement. The project allows for interesting design choices to be made.
    2) Medium: the work suffices but does not extend past the minimum.
    3) Easy: the project is simple, straightforward, and has little chance for meaningful design decisions.

3) Design of code (30/100)
    1) Great: Code is properly separated, abstracted, modular, and tested. Uses Rust features: traits and types: effectively and concisely.
       Code is documented and commented. Uses appropriate data structures.
    2) Subpar: Some abstraction, custom data types, error handling, modules. But not enough to represent excellent code.
    3) Terrible: if-else cascades, one giant function, one giant file.
4) Other factors for your final grade (10/100)
    1) Does you commit and comments from your partners reflect an appropriate amount of work?
