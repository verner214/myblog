my useful commands
git add .  -- markerar alla ändringar och nya filer som med i staging
git commit -m "obligatorisk kommentar" -- check init
git push -u origin master -- skickar till github



from start page after creating a new repository:

echo "# myblog" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/verner214/myblog.git
git push -u origin master