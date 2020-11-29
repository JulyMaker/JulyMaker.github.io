### Step 1

Use your-github-username.github.io as the new repo ( Replace your-github-username with yours).

### Step 2
```
 $ git clone https://github.com/yourusername/yourusername.github.io
 $ cd yourusername.github.io
 $ code .
 ```

### Step 3

 Open the files using VSCode and edit _config.yml and edit with your details:


```

    _config.yml file - replace with your own details
    _posts - Add your blog posts here
    _includes - You can replace the contents of the files with your data. (contains widgets)
    _assets/img - Add all your images here
```

### Step 4

 Install the development requirements:


    Git
    Ruby and Bundler
    VSCode

```
$ ruby -v
$ gem install bundler
$ bundler -v
$ bundle add jekyll
$ bundle exec jekyll -v
```

### Step 5

 Serve the site locally by running the following command below:

```
$ bundle exec jekyll serve --watch

or

$ jekyll serve
 ```

 Visit http://localhost:4000 for development server

### Step 5

Start populating your blog by adding your .md files in _posts. devlopr-jekyll already has a few examples.


Stylesheet : You’ll only work with a single file to edit/add theme style: assets/css/main.scss.

### Step 6

Once happy with your blog changes. Push your changes to dev branch.

```
 $ git add .
 $ git commit -m "my new blog using devlopr-jekyll"
 $ git push origin devBranch
```

### Step 7

Go to production md for more information