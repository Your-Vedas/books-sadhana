```
bundle install
ruby serve.rb
```

That will

1. combine the text with the template to generate a finished e-book in a new `build` directory, and
2. serve that finished e-book, which you can view at `http://localhost:8000/`.

To swap out the text, provide your own Markdown file and then edit `book.yaml`. The values there are mostly self-explanatory, and those that aren't probably need to be dropped or replaced.

The `serve.rb` script watches the entire `source` directory and, whenever you make a change, regenerates the e-book.

If you'd like to generate the e-book without starting a web server, you can just run `ruby generate.rb`.