# CIS198 Final Project

This is the final project for the class. The goal is for you to show your knowledge of Rust to implement, or contribute to Rust in a larger project than the homework allow.
Your project should play into the strengths of Rust. That is, you must show you effectively leveraged the features of Rust to the specific program. This can be for example though:
safety, typing (types and traits), low-level programming (e.g. processes and system calls), performance, or parallelism and concurrency
(see "Project Feature Requirements" below).

## Project Groups

Groups are of size 2-4.
Groups have been assigned and are posted on Piazza.

Each group will have a generated Github Repository for their project. Please use this repo to commit and work on your code.

At the end of the semester, you will have a chance to submit anonymous feedback about your teammates. If it is determined that work was not evenly distributed, this can affect the grades for teammates who did not do enough.

If someone in your group is being extremely unhelpful or unwelcoming, or you are having trouble working with your group and need a switch, let me know and we will work something out.

### Guidelines for working with your group

Please set up a communication channel and regular video meetings with your group.
Please make sure to meet at least weekly and ideally biweekly with your group -- there is not a lot of time left in the semester!

- For a communication channel, you can use Slack or another messaging platform like Discord, Messenger, etc.

- You can also re-use this as a way to get help in general, for example on Homework 4.

- This is particularly important since some of you may be working purely online (remotely).

## Requirements

### Project Feature Requirements

You will have a lot of leeway in choosing the final project, but in order to ensure your project involves some of the ideas of Rust, you should ensure that your project has at least **5 of the following 7 concrete features:**

- **Concurrency:** You satisfy this feature if you implement some form of concurrency (either multiple threads or multiple processes running in parallel). This can be for example, simply by optimizing one of your functions to run in parallel, or it could be a more fundamental part of your project, for example a program which profiles or runs other programs.
You can also satisfy this feature by using an external crate such as [`rayon`](https://docs.rs/rayon/1.5.0/rayon/).

- **System calls:** To satisfy this, implement some nontrivial interaction with the operating system through system calls. Plain file input/output doesn't count for this, but anything else does (e.g. spawning processes, executing commands, or any kind of network communication / web-related code).

- **Smart pointers:** To satisfy this feature, use at least one smart pointer features in Rust, other than `Box`: `Cell`, `RefCell`, `Rc`, `Arc`.

- **Data model** To satisfy this, your project should have at least one custom data structure that you implement that leverages Rust's type system, i.e. a struct which encapsulates data and methods of interest,
beyond just a simple wrapper.

- **Traits:** To satisfy this, define a custom trait that is relevant to your use case, and implement it for at least two different types (not just one). For example, you can use traits to define an interface or API, and then give different (competing) implementations of that API.

- **CLI:** Implement a CLI for your tool, using the `structopt` crate.

- **External Crates:** Use at least one new crate (on `crates.io`) that we have not seen in class. This should be for a specific purpose relevant to your project, e.g. web programming, machine learning, etc.

When you submit your project outline, choose which of the above features you are going for.

### Clippy and Rustfmt

Your project should have no warnings. You must use `cargo clippy` and `cargo fmt` to catch lints and to fix formatting.

### Unit Testing

Your project should include unit testing for all or most functions where it is possible. Logging is also a bonus, for functions that can't be unit testsed, but not strictly required.

## Proposal: Due Friday, April 16

You and your team must submit a proposal for a project. The proposal
is 5% of your grade in the course.

This should be a README file which describes your planned project.

Think of something exciting but not too ambitious -- you need to be able to complete it, with the number of group members you have, in about 3 weeks!

I will give you feedback about your chosen project. Your proposal does not have too be
long or detailed, but it must show that your team has a good idea for a project.
It should also show that you have thought about how to implement it, and how
to divide up work.
State which 5 of the 7 feature requirements you plan to satisfy,
and how.

## Final Project: Due May 11 (end of finals period)

The final project is an exercise in software engineering, design, and implementation. It is worth 20% of your course grade (separate from the 5% for the proposal)

## Examples of Projects

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

## Grading Rubric

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

4) Group sportsmanship (10/100)

  Did you have weekly video meetings with your group? Did everyone feel like they were included and had a say in the project and had ownership over their part of it?
