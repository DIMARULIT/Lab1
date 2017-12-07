[![https://a11yproject.com](https://a11yproject.com/img/README-logo.svg)](https://a11yproject.com)
# Contributing to A11Y Project
Do you enjoy web accessibility and want to help? **Here's how you can help.**

## Pattern Submissions
If you'd like to submit patterns to the A11Y Project make sure to do the following…

1. [Make a CodePen](https://codepen.io/pen) (or use an equivalent service like a JSFiddle or JSBin for example) **NOTE** : Please keep code as vanilla as possible. No Sass. No LESS. No HAML etc. You get the point.
2. [Submit your pen to our Issue Tracker](https://github.com/a11yproject/a11yproject.com/issues/new) w/the name of your pattern as the title.
3. Wait for the community to give you feedback and approval. **Note:** Keep the feedback and discussion to the pattern submitted and avoid discussing other patterns. Submit new patterns as separate issues.
4. “Git” down and boogie

    ![boogie dance](http://bukk.it/gitdown.gif)

## Writing Articles
We have a [list of articles](https://github.com/a11yproject/a11yproject.com/issues/12) we'd love to see written. Have an idea for an article? We'd love to know what you want to contribute.

1. Search to make sure someone hasn't snagged the article already.
2. Claim an article by starting a new issue with "Article: your title" as the issue title. The final title can (or probably should) be different.
3. When you check&ndash;in, reference that issue number in the commit, e.g., `re: #32`
4. Articles are written in plain text at a linkable location on the web. We recommend using GitHub's [gists](https://gist.github.com) (but [OK So Clap](http://oksoclap.com/) is another option if gists aren't your thing). Link us to your [gist](https://gist.github.com) (or your [clap](http://oksoclap.com/)) in the [issue field](https://github.com/a11yproject/a11yproject.com/issues) for your article and we'll be sure to clone and update our site accordingly with your masterpiece. When you are ready to submit the article via a pull request, we have a lovely [sample post file](_posts/example-post.md) to get you started.

### Plain-text Workflow for Article Submission
1. Make a [gist](https://gist.github.com) or a [clap](http://oksoclap.com/)
2. Start a conversation about it in an [issue](https://github.com/a11yproject/a11yproject.com/issues)
3. Roll the article in yourself via a pull request (gist only) **OR** ask someone to help you.

### Article Style Guide

Here are some suggestions and tips on writing your article:

- Short - Aim for a timed reading length of approximately two minutes.
- Focused - Keep it digestible and to a single topic. Articles that span multiple areas and topics are better broken up.

## Adding Resources

Find a great resource that you think will be useful to others?

- Add the url and title to the [resources](https://github.com/a11yproject/a11yproject.com/blob/gh-pages/_data/resources.yml) page under the appropriate category.

### Writing in YAML

YAML is a human readable markup language that's good for writing structured data. Even if you've never written anything in a .yml file, it shouldn't be too hard to understand the structure of the content. Yaml data is structured by spaces (you can not use tabs!), so an indented line means the content is nested within the parent.

For example, here is an ordered list:

```
- 'one'
- 'two'
- 'three'
```

Here is a dictionary, where each value has a name:

```
  thing1: 'a string value'
  thing2: 2
  thing3: 3
```

And here is how we could make the value of `thing1` a list:

```
thing1:
  - 'first'
  - 'second'
  - 'third'
```

For a full cheatsheet, you can visit the [official YAML site](http://yaml.org/about.html), or check out this [cheat sheet](https://cheat.readthedocs.io/en/latest/yaml.html).  

## Adding Events
Have an accessibility focused event you would like to promote?  Whether it's in person or online, you have two way you can get your event added to the project. Either [create a new issue](https://github.com/a11yproject/a11yproject.com/issues/new), or [edit the events.yml file](https://github.com/a11yproject/a11yproject.com/blob/gh-pages/_data/events.yml) directly and submit a pull request.

You'll want to add the following information about your event:
- Event title
- Date of event
- A brief description
- Web address (url) for more info
- Physical address of event (if applicable)
- Social Media Hashtag (if applicable)

## Reporting Issues
Notice something inaccurate? Noticed something inaccessible on this site? You think you can code something up better?

- File an issue.
- Preface your issue as either an `inaccuracy`, a `inaccessibility`, or a `bug` (for site issues) (e.g. "Bug: Link at archive not working").
- **ISSUES ARE NOT** free help on your website. Use [Stack Overflow](https://stackoverflow.com) for that.

## Stale Issues
An issue is considered in a "stale" state when the following conditions are met:

- Last comment was made over one year ago
- No movement since
- Not an open question
- Someone has attempted to address the issue, no comment from the author

When an issue has become stale a project maintainer will close the issue, leaving a note for the author to open a new issue if so desired.

## Key Branches

- `gh-pages` is the "master" branch. This is the website.

If you have a feature request(s) we suggest filing an issue initially to discuss your feature. Once that feature has been accepted you'll be off and running to feature making madness. Start a separate branch and use the following naming convention for your *feature branch*:

- `feature/name_of_feature`

## Build Process
- In order to create a site build you'll need to make sure you've run through all the listed commands in the order they appear from our [README.md](https://github.com/a11yproject/a11yproject.com#local-development)
- CSS changes must be done in ``.scss`` files first, never just the compiled files. We use [Codekit](http://incident57.com/codekit) to compile our *Sass* and *Compass*.


## Pull Requests

Filing a descriptive issue and then assigning it to yourself, before you send your request, will help in get your commit accepted. This way we'll have a better understanding of what your request entails and why it was made.

## To Set up Locally

You can take all the files of this site and run them just on your computer as if it were live online, only it's just on your machine.

### Requirements

* [Jekyll](https://jekyllrb.com/)
* [Ruby](https://www.ruby-lang.org/en/)
* [Git](https://git-scm.com/)

_If you have installed [GitHub Desktop](https://desktop.github.com), Git was also installed automatically._

To copy the repository's files from here onto your computer and to view and serve those files locally, at your computer's command line type:

```bash
git clone https://github.com/a11yproject/a11yproject.com.git
cd a11yproject.com
script/bootstrap
script/server
```
Open `http://localhost:4000` in your browser

## License

By contributing your code, you agree to license your contribution under the terms of the [APLv2](http://www.apache.org/licenses/LICENSE-2.0.html).
