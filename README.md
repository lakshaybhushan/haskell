# Haskell MOOC Solutions

This repository contains my solutions to the Haskell MOOC course offered by the University of Helsinki.
[Course page](https://haskell.mooc.fi)


## About the course

This is an online course on Functional Programming that uses the
Haskell programming language. You can study at your own pace. All the
material and exercises are openly available.

The course is intended to be followed through the [Course page](https://haskell.mooc.fi), but in case the course page is down or you want an offline backup, the course material is also available in this repository ([part1.html](part1.html), [part2.html](part2.html)).

## My Solutions

My solutions to the course exercises can be found under the `exercises/` directory. All required dependencies
can be downloaded and built with:

```
stack build
```

The exercises are Haskell source code files named `Set1.hs`, `Set2.hs` and so on. I have completed the exercises by editing the files according to the instructions in each file. You can check the solutions by running

```
stack runhaskell SetXTest.hs
```

in the `exercises/` directory. Remember to replace `X` with the number
of the set you are working on.

See [the material](part1.html#working-on-the-exercises) for more info.

## Troubleshooting

Here are some fixes for common problems with `stack build`:

- If you get an error like `While building package zlib-0.6.2.3`, you need to install the zlib library headers. The right command for Ubuntu is `sudo apt install zlib1g-dev`.
- If you get an error like `Downloading lts-18.18 build plan ... RedownloadInvalidResponse`, your version of stack is too old. Run `stack upgrade` to get a newer one.