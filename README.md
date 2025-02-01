git init
git add .
git commit -m "First commit"
git branch -M main
git remote add origin https://github.com/SalahPS7/Test.git
git push -u origin main

git checkout -b gh-pages
git rm -rf .
cp -r build/web/* .
git add .
git commit -m "Deploy Flutter Web"
git push -u origin gh-pages
