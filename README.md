# Welcome to Fountain-cookiecutter - a cookiecutter template for starting a Fountain screenplay!

This repository is a template repository (a cookiecutter) that allows you to quickly set up a new [Fountain](https://www.fountain.io) screenplay project.


## Features

  * Very simple, configurable setup of a fully functional project
  * Automatically performs a Git repository setup
  * Based on an established tool: [Cookiecutter](https://github.com/cookiecutter/cookiecutter) has >17k stars on Github!


## Prerequisites

In order to use Fountain-cookiecutter template for your next Fountain screenplay, you need the following software installed:

  * Python `>= 3.6`
  * [Cookiecutter](https://github.com/cookiecutter/cookiecutter) e.g. by running `pip install cookiecutter`.
  * Git `>= 1.8.2`
  * Wrap `>= 0.3.1`


## Using Fountain-cookiecutter - a cookiecutter template for Fountain screenplays

Simply run the cookiecutter command line interface:

```
cookiecutter gh:calligraffiti/fountain-cookiecutter
```

This will start an interactive prompt that will configure and generate your screenplay project.
One of the prompts will ask you for a remote repository URL, so you should head to
the Git hosting service of your choice and add a new empty repository e.g. [on Github](https://github.com/new).


## Git Repository

Cookiecutter automatically initializes, adds and commits, your local files to Git with the commit message 'initial commit'. You're ready to begin editing your `project_name.fountain` file and start using git right away!

If you're new to Git concider searching [getting started with git](https://duckduckgo.com/?q=git+getting+started&ia=web), or visit W3 Schools '[Git Getting Started](https://www.w3schools.com/git/git_getstarted.asp).'

***Note:*** .PDF files are not tracked by Git in this repo. Tracking PDF files just adds unnecessary bloat to your project repository, and really it's just a render. It's the `.fountain` file that matters most.


## Configuration

This cookiecutter accepts the following configuration options:

  * `project_title`: The human-readable name of your screenplay, defaults to `Screenplay Title`
  * `remote_url`: The remote URL for the newly created repository. This is not only used to add it as a remote to the Git repository, but also to enable integration with some services. Defaults to `None` although we strongly advise you to specify it.
  * `project_slug`: This will be the name of the generated directory.By default, it is deduced from the specified remote URL and the given project name.
  * `full_name`: Author's name, defaults to `Your Name`.
  * `prod_company`: Production company name, defaults to `None`.
  * `email`: Author's email, defaults to `Your Email`.
  *  `prod_addr1`: Contact address 1, author, or production companies street address. `Example: 321 John St., Ste. 7"`
  *  `prod_addr2`: Contact address 2, author, or production companies city and state. `Example: City, State & Zip: example: Nyak, NY 10960`
  *  `year`: Year written, defaults to current year.
  *  `date`: Formatted date, defaults to current date.
  * `license`: Adds a license file to the repository. It can be chosen from `Proprietary`, US Copyright ***(default)***, a  `CC_BY-NC-ND_4.0` - ***[Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/)***, or a `CC_BY-SA_4.0` - ***[Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/)***. It can also be left to `None` which will produce a simple copyright statement.

If you are using `fountain-cookiecutter` a lot, you can customize your default values by providing a `.cookiecutterrc` file in your home directory, for more details see the [cookiecutter documentation](https://cookiecutter.readthedocs.io/en/latest/advanced/user_config.html).


## Script Writers Font

We recommend installing [Curier Prime](https://quoteunquoteapps.com/courierprime/), an open SIL licensed typeface, designed by Alan Dague-Greene, specifically for screenplays. This is the default font `Wrap` looks for when rendering your script.


## Rendering Your Script

We recommend using [Wraparound](https://wraparound.github.io/) to render your Fountain files to PDF or HTML. It really is the best we have tested for creating professionally formatted screenplays. It does not currently render out to FinalDraft, .FDX file format. FinalDraft does now support the import of `.fountain` files, but if you do need to export a Fountain screenplay to .FDX because the format is required by production, we recommend using a tool like [`scripttool`](https://rsdoiel.github.io/scripttool/) or [AfterWriting](https://afterwriting.com/).

To render your screenplay using Wrap just use `wrap` | the format you wish `pdf` or `html` | and the file name `proj_name.fountain` or `proj_name.wrap`. E.g.:
```
wrap pdf proj_name.fountain
```
The above command will out-put your PDF file into the same directory. If you wish to output do a different directory, or give it another name just use the `--out` flag. E.g.:
```
wrap pdf proj_name.fountain --out proj_name-v2.pdf
```

## File Structure

├── LICENSE.md                          // License info for your project
├── README.md                           // README for your repository
├── TODO.md                             // Infor on next steps for your repository
├── untracked_files                     // A folder for files you do not wish tracked by Git
│   ├── README.md                       // How to use this directory
│   ├── notes                           // A dir for notes and research, not tracked by Git
│   └── templates
│       ├── character_profile_main.md   // A character profile template for a main character
│       ├── character_profile_xtra.md   // A character profile template for a lesser character
│       └── setting_template.md         // A scene setting profile template
└── proj_name.fountain                  // Your screenplay


## Contribute!
Please do help improve this cookiecutter! Submit pull requests to this repository, or if you notice any bugs, please report them using [the Github issue tracker](https://github.com/calligraffiti/fountain-cookiecutter)


### Credits
Special thanks to [Dominic Kempf](https://github.com/dokempf) for making the [meta-cookiecutter](https://github.com/dokempf/meta-cookiecutter) template that got this here fountain.cookiecutter started at full steam.