# How to update for a new semester

1. In the `static/files/` directory, add a folder for the semester, e.g. `static/files/2022/02/`. Then create a subdirectory for each syllabus. Tip: copy an existing course directory.
2. Edit the home page content in `content/authors/admin/_index.md`. (I have not figured out how to revise the &lt;h3&gt; element on that page so fix it in `themes/academic/layouts/partials/widgets/about.html`.)
3. Add a new filter in the file `projects.md`.

Check the site by setting the working directory to `academic-kickstart-master/` and then executing the command `hugo server -D`. Look for errors. Test the links in a browser at http://localhost:1313.
It's probably a good idea to make a backup copy before generating the site using the command `hugo -D`. The generated files are placed in the `public/` directory.
Manually edit the &lt;h3&gt; element on the home page: `public/index.html`.
Upload the generated site to GitHub in repository `sykesda/sykesda.github.io`. Using the GitHub app makes this easier. Make `public` the working directory and then `cp -R * /Users/sykesda/Documents/GitHub/sykesda.github.io`. Files that were changed should be pushed to GitHub.
Check out the site at `https://sykesda.github.io`.