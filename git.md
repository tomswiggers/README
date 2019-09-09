
# Point branch develop to HEAD of HEAD of master branch

git checkout -B develop master
git push -f

# Pull after forced push

git fetch origin
git reset --hard origin/develop

# Delete branch

git branch -d v60
git push --delete origin v60
