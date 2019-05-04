--------- enkelt cms --------- 
kommandon: buildblog.bat
copy header.html + /blog1/body.html + footer.html /blog1/index.html
copy header.html + /blog2/body.html + footer.html /blog2/index.html

--------- filer ------------
/src/blog1/body.html
/src/blog1/localimage1.jpg
/src/blog1/localimage2.jpg
/src/blog2/etc.
/images/
/js/
/css/
header.html
footer.html
about.html
404.html

--------------- output, laddas upp till molnet -------------
/src/blog1/index.html -- .gitignore
/src/blog2/index.html -- etc.


my useful commands
git add .  -- markerar alla ändringar och nya filer som med i staging
git commit -m "obligatorisk kommentar" -- check init
git push -u origin master -- skickar till github
git clone https://github.com/verner214/myblog.git


from start page after creating a new repository:

echo "# myblog" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/verner214/myblog.git
git push -u origin master