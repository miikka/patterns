# Code review

1. Review the code, not the people.
2. Review what computers can’t review.
3. Give constructive feedback.
4. Praise good work.
5. Everybody can and should review everybody’s code.
6. Stay humble.


## Why review?

* To find bugs and to improve the design.
* To cultivate a common style.
* To spread knowledge about the code.
* To educate both the author and the reviewer.

Does it work? My gut feeling is that quite well for spreading knowledge and not
so well for finding bugs. I haven't searched the literature.

## Comment tags

Sometimes I prefix my code review comments with a `[tag]` to indicate the nature
of the comment. The most common tags are:

* `[nit]`: There is something small to be changed, but it's so trivial that
  merging this patch without change it is okay.
* `[minor]`: I know I'm asking for a trivial change, but it really needs to be
  done before the patch can be merged.

For example, pointing out a typo in a comment is a `[nit]`, whereas requesting
more information to an error message might be a `[minor]`.


## Misc.

If the code disagrees with its comments, that's a bug and the patch can't be
merged. One way to fix this is to remove the comments.
