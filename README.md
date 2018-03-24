# termdash

This project implements a terminal based dashboard. The feature set is inspired
by the [gizak/termui](http://github.com/gizak/termui) project, which in turn
was inspired by a javascript based
[yaronn/blessed-contrib](http://github.com/yaronn/blessed-contrib). Why the
rewrite you ask?

1. The above mentioned [gizak/termui](http://github.com/gizak/termui) is
   abandoned and isn't maintained anymore.
1. The project doesn't follow the design goals outlined below.
1. The project is released under a licence I cannot use.

# Design goals

This effort is focused on good software design and maintainability. By a good
software I mean:

1. Write readable, well documented code.
1. Only beautiful, simple APIs, no exposed concurrency, channels, internals, etc.
1. Follow [Effective Go](http://golang.org/doc/effective_go.html).
1. Provide an infrastructure that allows development of individual dashboard
   components in separation.
1. The infrastructure must enforce consistency in how the dashboard components
   are implemented.
1. Focus on maintainability, the infrastructure and dashboard components must
   have good test coverage, the repository must have CI/CD enabled.

On top of that - let's have fun, learn something and become better developers
together.

# Requirements

1. Apache-2.0 licence for the project.
1. Tree based container for placing dashboard elements.
1. Mouse and keyboard input.
1. Cross-platform terminal based output.
1. Unit testing framework for simple and readable tests of dashboard elements.