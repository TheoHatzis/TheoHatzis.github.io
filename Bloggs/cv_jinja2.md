# Profile in YAML 

The following snippet 

```
def do_all(yam_path, pth_template, outfile):
    context = {}
    cfg = {}

    for filename in os.listdir(yam_path):
        if filename.endswith(".yaml"):
            cfg.update(yaml.load(open(fr'{yam_path}\\{filename}'), yaml.SafeLoader))
            context['cfg'] = cfg

    with open(f'{outfile}', 'w') as f:
        f.write(Template(open(pth_template).read()).render(context))

```



```
{% set elv = cfg['elevator'] %}
{% set a1 = elv['personal details'] %}
{% set s1 =elv['short_careerbio'] %}
{% set j1 = elv['roles'] %}
{% set s2 =cfg.linkedin_aboutme %}
{% set linked =cfg['cv_related']['linkedin']  %}

# {{a1.name}}

{%- if a1.addr_header == 1 %}

### {{a1.address}}    {{a1.email}}    {{ a1.phone}}
{% else %}

### {{a1.email}}    {{ a1.phone}}
{% endif %}


# {{s1.0}}

{{s1.0}}
{%- if linked == 0 %}
{{s1.1}}

{{s1.2}}

{{s1.3}}
{%- else %}

{{s2.1}}

{{s2.2}}

{%- endif %}

# Project Interests:
{% for keys, values  in j1.items():  %}

## {{ keys}}
{% for ii, oo in values.items() %}

* {{oo}}
{% endfor %}
{% endfor %}

# Experience Areas:
{% set h1 = elv['experience_areas'] %}

{% for keys, values  in h1.items():  %}

## {{keys}}
{% for ii, oo in values.items() %}

* {{oo}}
  {% endfor %}
  {% endfor %}

# {{cfg.cv_related.f_items1.train_edu}}
{% for ii in cfg['Training'].values() %}
* {{ii}}
{% endfor %}


# {{cfg.cv_related.projects2}}
{% for ii in cfg.cv_related.projectss.values():  %}

* {{cfg[ii].role}}, {{cfg[ii].company }}, {{cfg[ii].start_date}} - {{cfg[ii].end_date}} [{{cfg[ii].agent1}}]
    * {{cfg[ii].exp_short.k1}}

{% endfor %}
```



