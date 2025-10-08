https://www.haskell.org/get-started/

Writing your first Haskell program
In your editor, create a new file named hello.hs. Write the following in it:

main = do
  putStrLn "Hello, everybody!"
  putStrLn ("Please look at my favorite odd numbers: " ++ show (filter odd [10..20]))
You can now compile it with ghc to produce an executable called hello that we will then run:

> ghc hello.hs
> ./hello
Hello, everybody!
Please look at my favorite odd numbers: [11,13,15,17,19]
There you go, you just wrote a short, polite program in Haskell!

GHCI TIP: You can also load your file directly into ghci, which will enable you to play with any functions and other definitions you defined in it. So for our example, we can just load hello.hs with GHCi and then call the function main like this:

> ghci hello.hs
GHCi, version 8.10.7: https://www.haskell.org/ghc/  :? for help
[1 of 1] Compiling Main             ( hello.hs, interpreted )
Ok, one module loaded.
> main
Hello, everybody!
Please look at my favorite odd numbers: [11,13,15,17,19]