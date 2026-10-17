# m01l04-02 · The bootstrap script, part one: settings

**Lesson:** [Bootstrap A Local Cluster And Check Your Context](https://learnsome.tech/learn/kubernetes-course/m01l04) (lesson 1.4, module 1: The Cluster And Your First Diagnosis) · Free  
**Check:** Read along

## Goal

You can create a throwaway local cluster with kind or minikube, read a kubeconfig as three separate lists, prove which cluster and namespace a command will hit before you run it, and keep the course cluster in a kubeconfig of its own.

## Files

- [`starter/m01-create-cluster.sh`](starter/m01-create-cluster.sh): the listing from the lesson
- [`check.json`](check.json): how `./check` runs and checks this lab

## Steps

1. Read `starter/m01-create-cluster.sh` alongside the lesson.
2. Follow it the way the lesson builds it:
   - Lines 1–7: the header says what it is for
   - Lines 8–13: four settings
   - Lines 14–16: a small helper
3. Notes from the lesson:
   - Line 11: a kubeconfig of its own: this is the safety property
   - Line 12: pinning the node image pins the Kubernetes version

## How to check

**Read along.** It is a listing to read alongside the lesson, not a program to run.

There is nothing to check: `./check m01l04-02` says so and moves on.

---

[Open the lesson on LearnSome.tech](https://learnsome.tech/learn/kubernetes-course/m01l04) · [All labs of this lesson](../README.md) · [Course README](../../../README.md)
