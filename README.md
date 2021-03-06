# Job Interview

[![Build Status](https://secure.travis-ci.org/ruby-jokes/job_interview.png?branch=master)](http://travis-ci.org/ruby-jokes/job_interview)

## SYNOPSIS

Let's face it. Programming job interviews can be annoying. And sometimes the questions require you to actually think. With Job Interview, most programming interview questions can be answered in 3 lines of Ruby.

## USAGE

    require 'job_interview'
    @answer = JobInterview::Answer.new

    @answer.fizz_buzz(5)
    => [1, 2, "Fizz", 4, "Buzz"]

    @answer.fib(10)
    => [1, 1, 2, 3, 5, 8, 13, 21, 34, 55]

    @answer.quine(__FILE__)
    => "@answer.quine(__FILE__)"

    @answer.primes(10)
    => [2, 3, 5, 7, 11, 13, 17, 19, 23, 29]

Now, job_interview will help you answer non-technical interview questions as well! Simply call the appropriate method, and a randomly constructed answer will pop out.

    include JobInterview::Questions

Q. Where do you see yourself in five years?

    in_five_years

    => "I'd like to have made someone else rich with my re-contextualized non-volatile open architecture."

Q. Why are you leaving your current position?

    leaving_current

     => "I'm seeking to optimize extensible applications."

Q.  Why are manhole covers round?

    manhole_cover

     => "Because Reuleaux Triangles are hard to manufacture."

Q.  What is you greatest weakness?

    greatest_weakness

     => "I always fail so rarely so I make too much money."

Q. Why do you want to work here?

    why_here

    => "Your company has revolutionized seamless next generation interface."

Q. Does P = NP?

    p_equals_np

    => "I doubt it, but it would make life easier for traveling salesmen."

## FAQ

  Q. Why would you even do this?

  A. We wanted to hack on something trivial and silly at BohConf 2012. Also, most job interviews are dumb, and we felt the need to point this out.

  Q. Do you expect this of be of any use to anyone, ever?

  A. No.

  Q. So what's next?

  A. The Ruby implementation of job_interview is pretty decent at this point, we think. But maybe you're not applying for a Ruby job. So a Clojure implementation seems likely, possibly to be followed by JavaScript.

## AUTHORS

[Micah Gates](https://github.com/mgates)

[Jason Lewis](https://github.com/canweriotnow)

The authors would also like to thank:

- That one fellow we promised we'd put here, before we forgot his name (If you're him, let us know)

## LICENSE


Copyright (C) 2012 Micah Gates and Jason Lewis

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
