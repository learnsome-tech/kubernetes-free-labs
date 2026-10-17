# m01l04-07 · Selecting the course cluster in a new shell

**Lesson:** [Bootstrap A Local Cluster And Check Your Context](https://learnsome.tech/learn/kubernetes-course/m01l04) (lesson 1.4, module 1: The Cluster And Your First Diagnosis) · Free  
**Check:** Read along

## Goal

You can create a throwaway local cluster with kind or minikube, read a kubeconfig as three separate lists, prove which cluster and namespace a command will hit before you run it, and keep the course cluster in a kubeconfig of its own.

## Files

- [`starter/m01-use-cluster.sh`](starter/m01-use-cluster.sh): the listing from the lesson
- [`check.json`](check.json): how `./check` runs and checks this lab

## Steps

1. Read `starter/m01-use-cluster.sh` alongside the lesson.
2. Follow it the way the lesson builds it:
   - Lines 1–3: the comment is the important line
   - Lines 4–5: prints the context back
3. Notes from the lesson:
   - Line 4: the variable can name several files, separated by colons

## How to check

**Read along.** It is a listing to read alongside the lesson, not a program to run.

There is nothing to check: `./check m01l04-07` says so and moves on.

---

[Open the lesson on LearnSome.tech](https://learnsome.tech/learn/kubernetes-course/m01l04) · [All labs of this lesson](../README.md) · [Course README](../../../README.md)
