This is a cheat sheet for the Jinja templating syntax.

## Syntax
The syntax is somewhat similar to ERB except for {} instead of <> quotes
```jinja
{% raw %}
     {{ ... }}           # Escaping for expressions that create output
     {% ... %}           # Escaping for control statements
     # ... ##            # Line statements
{% endraw %}
```


## Loops
```jinja
{% raw %}
     {% for i in list %} ... {% endfor %}
{% endraw %}
```

## Functions
Defining functions
```jinja
{% raw %}
     {% macro myfunct(param1, param2) %}
     ...
     {% endmacro %}
{% endraw %}
```

Using functions
```jinja
{% raw %}
     {% myfunc(var, 5) %}
{% endraw %}
```
