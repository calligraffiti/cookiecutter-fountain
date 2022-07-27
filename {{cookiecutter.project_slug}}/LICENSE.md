Copyright (c){% now 'utc', '%Y' %}, {% if cookiecutter.prod_company == 'None' -%}{{ cookiecutter.full_name }}{%- else -%}{{ cookiecutter.prod_company }}{%- endif %}
{% if cookiecutter.license == "Proprietary" %}
This work is protected under the copyright laws of the United States and other countries throughout the world. Country of first publication: United States of America. Any unauthorized distribution, or copying of this manuscript or any part thereof may result in civil liability and criminal prosecution. The story, all names, characters, and incidents portrayed in this work are fictitious. Copyright ©{{ cookiecutter.year }} {% if cookiecutter.prod_company == 'None' -%}{{ cookiecutter.full_name }}{%- else -%}{{ cookiecutter.prod_company }}{%- endif %}. All rights reserved.
{% endif %}
{% if cookiecutter.license == "CC_BY-NC-ND_4.0" %}
## Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License.

This work is licensed under an Attribution-NonCommercial-NoDerivs 4.0 International license (CC BY NC ND 4.0). This license allows reusers to copy and distribute the material in any medium or format in unadapted form only, for noncommercial purposes only, and only so long as attribution is given to the creator. Attribution should include the following information:
{{ cookiecutter.full_name }}, {{ cookiecutter.project_title }}

Further details about CC BY-NC-ND licenses are available at http://creativecommons.org/licenses/by-nc-nd/4.0/
or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
{% endif %}
{% if cookiecutter.license == "CC_BY-SA_4.0" %}
## Creative Commons Attribution-ShareAlike 4.0 International License.

This work is licensed under an Attribution-ShareAlike 4.0 International (CC BY-SA 4.0). This license allows reusers to share — copy and redistribute the material in any medium or format, adapt — remix, transform, and build upon the material for any purpose, even commercially. Attribution should include the following information:
{{ cookiecutter.full_name }}, {{ cookiecutter.project_title }}

Further details about CC BY-SA 4.0 licenses are available at http://creativecommons.org/licenses/by-sa/4.0/
or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
{% endif %}