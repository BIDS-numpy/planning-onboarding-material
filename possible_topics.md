# Possible topics for video content

This document aims to collate possible ideas/outlines for video content related
to onboarding (or otherwise encouraging) NumPy developers.

## Numpy basics

Opening the call for people to film the tutorials they submitted on
[numpy/numpy-tutorials](https://github.com/numpy/numpy-tutorials). Of course
only a subset would be willing, but hopefully their video would encourage more
people to join and submit tutorials. And even more hopefully, the `tutorial ==>
development` pipeline would 'activate'.

## Workflow basics

Start with the basic `git`/`github` workflow
 - Fork, clone, set upstream

Then on to setting up an environment
 - There are a lot of options here (`conda`, `venv`, etc.) How to deal with the
   various options?
	* Personally, I like `venv` as it's Python standard library
	  and doesn't require any special knowledge of package managers
 - Highlight the way `numpy` recommends doing it with the
   `{test/doc}_requirements.txt` files.

Installing numpy
 - Again, various ways of doing it with their own advantages/disadvantages.
   How to deal with the options? Is there a **right** way?
	 * Various `setupy.py` options (`install`, `develop`, `build_ext`, etc)
	 * `pip` and/or `conda`

## Documentation build

An obvious extension of `Workflow basics`, but has enough nuances to perhaps be
its own separate thing (depending on how long/detailed the first is).  For
example:
 - doc building checks the git hash, won't build if the current commit
   differs from the installed version
 - How to run doctests with `tools/refguide_check.py`?

Walking through a documentation PR would be an obvious example, but maybe a
separate video? Or could go into this one.

## Running tests locally

A video on `runtests.py` and the various features? Actually has a lot of
(not-heavily-used) functionality like performing benchmarks with `asv` and
type-checks with `mypy` (pretty new).

## The full PR walkthrough

Again, it's not clear to me where the boundaries between this video and other
potential topics are, but it seems appealing to have a full walkthrough of
"putting all the pieces together" and submitting a PR.

It would be *really* nice if this included the back-and-forth of the review
process (which very often tends to be pretty extensive), but this might be very
difficult to capture in a video.
