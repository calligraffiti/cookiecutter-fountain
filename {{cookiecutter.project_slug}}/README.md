# {{ cookiecutter.project_title }}

A screenplay by {{ cookiecutter.full_name }}

---

## Fountain
This screenplay is written in [Fountain](https://www.fountain.io), a free and open-source Markdown like syntax for screenwriting. If you are new to Fountain and would like to contribute to this project, please visit the [Fountain Syntax documentation](https://fountain.io/syntax) page to learn more. Many [writing apps](https://fountain.io/apps) support the `.fountain` file format. You may already be using one of them.


## Script Writers Font

We recommend installing [Curier Prime](https://quoteunquoteapps.com/courierprime/), an open SIL licensed typeface, designed by Alan Dague-Greene, specifically for screenplays. This is the default font `Wrap` looks for when rendering your script. If it's not available on your system Wrap will default to Curier.


## Rendering Your Script

We recommend using [Wraparound](https://wraparound.github.io/) to render your Fountain files to PDF or HTML. It really is the best we have tested for creating professionally formatted screenplays. It does not currently render out to FinalDraft, .FDX file format. FinalDraft does now support the import of `.fountain` files, but if you do need to export a Fountain screenplay to .FDX because the format is required by production, we recommend using a tool like [AfterWriting](https://afterwriting.com/) or [Fountain Loader](https://fountainloader.com/).

To render your screenplay using Wrap just use the `wrap` command | the format you wish `pdf` or `html` | and the file name `proj_name.fountain` or `proj_name.wrap`. E.g.:
```
wrap pdf proj_name.fountain
```
The above command will out-put your PDF file into the same directory you are currently in. If you wish to output do a different directory, or give it another name just use the `--out` flag. E.g.:
```
wrap pdf proj_name.fountain --out proj_name-v2.pdf

---

{% if cookiecutter.license == "None" -%}
Copyright (c){{ cookiecutter.year }}, {{ cookiecutter.full_name }}. All rights reserved.
{% endif -%}
{% if cookiecutter.license == "Proprietary" -%}
Copyright (c){{ cookiecutter.year }}, {% if cookiecutter.prod_company == 'None' -%}{{ cookiecutter.full_name }}{%- else -%}{{ cookiecutter.prod_company }}{%- endif %}. All rights reserved.
{% endif -%}
{% if cookiecutter.license == "CC_BY-NC-ND_4.0" -%}
[![CC BY-NC-ND 4.0](https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-nd/4.0/) <br>
This work is licensed under a Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License
{% endif -%}
{% if cookiecutter.license == "CC_BY-SA_4.0" -%}
[![CC BY-SA 4.0](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-nc-nd/4.0/) <br>
This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.
{% endif -%}
{{ "\n" -}}