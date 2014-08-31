Test what happens when a pull request has tons of commits.

Branch `a` will me merged into master (fast forward) with tons of commits.

    git checkout -b a
    for i in {1..1000}; echo $i; do touch $i; git add $i; git commit -m $i; done
