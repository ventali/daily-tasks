# daily-tasks

- [11162023]

01

https://github.com/lita-xyz/llvm-valida/issues/3

I've worked on issue #3, but only up to the point of creating and running a smoke test. What I did not do was add that smoke test to the LLVM test suite. It is committed to our fork of the LLVM test suite, in the develop branch, but the running of it is not automated as part of running the LLVM test suite.

A good starting point on this issue would be to write a shell script, committed to our fork of the LLVM test suite, which runs the test cases we have added in our develop branch. My comment here provides an example of how we are running those tests: https://github.com/lita-xyz/llvm-valida/issues/4#issuecomment-1777460382

What would be even nicer would be if our tests ran inside the LLVM test harness. A further step after that would be if the pre-existing LLVM test suite ran against the Valida backend, to the extent that that makes sense. It's not obvious to me how to arrange for either of these things, since we rely on external programs, valida to run the code and valida-asm to assemble the assembly code output by LLVM. So I'm not sure how practical it is to take these next steps at this point, and perhaps a simple shell script to run our tests is all that we need at this point on automating our test suite.

02

https://github.com/lita-xyz/llvm-valida/issues/19

https://github.com/lita-xyz/llvm-valida/issues/24



