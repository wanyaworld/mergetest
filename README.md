# mergetest
for merge commit test

what i learned:
if we checkout or reset to merge commit,
we're going to the state the branch is made (which can be very old state)
if we checkout or reset to HEAD~n
merge commits do not consume "n"
for example, suppose the following situation:
head -> merge-commit-a -> commit-b -> merge-commit-c -> commit-d

if we checkout HEAD~1, we go to commit-b, not a, since merge-commit-a do not consume n

what the ..
