# first time
git clone git@github.com:fathom-global/OasisLMF-GFC.git
cd OasisLMF-GFC/
git checkout main
git checkout -b dev
git push --set-upstream origin dev
git remote add upstream https://github.com/OasisLMF/OasisLMF.git
git fetch upstream

# merge a PR
git fetch upstream pull/1838/head:pr-1838
git checkout dev
git merge pr-1838
git push

2026-01-29: cloned
2026-01-29: branched dev from main
2026-01-29: merged PR #1838 into dev
2026-01-30: merged PR #1846 into dev
2026-02-09: merged PR #1868
2026-02-10: changed "RUNNING" message in utils/log.py to "RUNNING (Fathom-oasislmf)"
